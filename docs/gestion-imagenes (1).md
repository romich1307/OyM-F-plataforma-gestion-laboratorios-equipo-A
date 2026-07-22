# Gestión de Imágenes y Trazabilidad

## Flujo Principal

1. Solicitud de imagen (Proyecto o Curso)
2. Búsqueda automática en Harbor
3. Si no existe → Responsable revisa y aprueba creación
4. Escaneo de vulnerabilidades (Trivy)
5. Firma de imagen
6. Publicación con metadatos de trazabilidad
7. Estudiantes pueden descargar la imagen oficial
8. Actualizaciones controladas *(ver "Mantenimiento y Actualización" más abajo)*

**Beneficio clave:** Los alumnos trabajan con el **mismo entorno** dentro y fuera del laboratorio.

> **Qué se mejora respecto al documento original:** se agrega el paso 8. El flujo original terminaba en el paso 7 y no contemplaba qué pasa con una imagen después de publicada.
> **Justificación:** sin este paso, una imagen con una vulnerabilidad descubierta después de su publicación podía quedar en uso indefinidamente sin ningún mecanismo de corrección.

---

## Política de Seguridad: "Fail the Build"

> **Sección nueva — no existía en el documento original.**
> **Justificación:** el flujo original no definía qué ocurría si Trivy encontraba una vulnerabilidad crítica, dejando la decisión a criterio informal del responsable en el momento.

- Cualquier vulnerabilidad de severidad **crítica o alta** detectada por Trivy **bloquea automáticamente** la publicación de la imagen.
- **Única excepción:** aprobación explícita y documentada del Chapter Lead de Seguridad, únicamente en casos de urgencia académica justificada (ej. imagen requerida para una práctica de esa semana sin alternativa).
- Toda excepción debe quedar registrada con: motivo, responsable que aprueba, y fecha límite de remediación.

---

## SLA de Aprobación

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no existía un tiempo de respuesta comprometido para la revisión manual, lo que podía convertir ese paso en un cuello de botella si un docente necesitaba una imagen con poca anticipación.

| Paso | Responsable | SLA |
|---|---|---|
| Revisión y aprobación de creación de imagen | Responsable de Imágenes | ≤ 5 días hábiles |
| Solicitud de imagen nueva por parte de un docente | Docente | Debe abrirse con ≥ 2 semanas de anticipación a la práctica |
| Escaneo de vulnerabilidades | Automático (Trivy) | ≤ 1 hora |
| Re-escaneo periódico de imágenes activas | Automático | Mensual |

---

## Firma Digital y Verificación

> **Sección nueva — no existía en el documento original.** El documento original solo decía "Firma de imagen" (paso 5) sin ningún detalle técnico.
> **Justificación:** no se especificaba el mecanismo de firma ni cómo se verifica en las computadoras personales de los estudiantes, fuera del control del laboratorio.

- **Mecanismo de firma:** Cosign/Sigstore.
- **Verificación en el clúster:** políticas de admisión (admission control) en Kubernetes que rechazan imágenes sin firma válida.
- **Verificación en equipos personales de estudiantes:** el script oficial de descarga debe incluir la verificación de firma como paso obligatorio, de modo que la seguridad no dependa del control administrativo del laboratorio.

```bash
# Ejemplo de verificación en el script de descarga
cosign verify --key cosign.pub harbor.universidad.edu/curso-bd:2026-1
```

---

## Política de Versionado

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no existía una política de versionado, un vacío crítico para la reproducibilidad de una práctica o proyecto evaluado si la imagen "oficial" cambia en un semestre posterior.

- **Versionado inmutable por semestre:** formato `curso:AAAA-S` (ej. `curso-bd:2026-1`).
- **Prohibido el uso de `latest`** en imágenes usadas para prácticas o proyectos evaluados, para garantizar la reproducibilidad del entorno en el que un estudiante fue evaluado.
- Cada nueva versión de una imagen genera un tag nuevo; no se sobrescriben tags existentes.

---

## Política de Retención

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no había ninguna regla sobre qué hacer con imágenes de semestres anteriores, lo que podía derivar en acumulación indefinida de imágenes sin mantenimiento de seguridad.

- Se conservan las **últimas 3 versiones estables** de cada imagen por curso.
- Las versiones anteriores se archivan (almacenamiento frío) y se eliminan del registro activo tras 6 meses sin uso.
- Las imágenes de semestres anteriores sin actividad se marcan para revisión antes de su descarte definitivo.

---

## Mantenimiento y Actualización de Imágenes Publicadas

> **Sección nueva — no existía en el documento original.**
> **Justificación:** el flujo original solo cubría la creación inicial de una imagen, sin contemplar cómo se actualiza una imagen ya publicada (ej. ante un parche de seguridad), lo que podía dejar cursos completos usando una imagen vulnerable durante meses.

1. Detección de nueva versión de una dependencia base (ej. mediante Renovate/Dependabot).
2. Re-escaneo automático mensual de todas las imágenes activas en Harbor.
3. Si se detecta una vulnerabilidad nueva en una imagen ya publicada:
   - Notificación automática al Responsable de Imágenes.
   - Se aplica la política de "Fail the Build" para bloquear su uso en nuevas descargas hasta remediar.
4. Publicación de la imagen corregida bajo un nuevo tag inmutable (no se sobrescribe la versión anterior, para no romper reproducibilidad de trabajos ya evaluados).
5. Notificación a los usuarios activos de esa imagen sobre la disponibilidad de la corrección.

---

## Matriz RACI

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no quedaba claro quién era "el Responsable" en cada paso del proceso (¿docente, equipo de plataforma, seguridad?), ambigüedad que podía generar demoras entre distintos actores universitarios.

| Actividad | Docente | Responsable de Imágenes | Chapter Lead Seguridad | Estudiante |
|---|---|---|---|---|
| Solicitud de imagen | R | I | I | C |
| Aprobación de creación | C | A/R | C | I |
| Escaneo de vulnerabilidades | I | R | A | I |
| Excepción a "Fail the Build" | C | C | R/A | I |
| Publicación | I | R | A | I |
| Verificación de firma en descarga | I | I | A | R |
| Re-escaneo periódico | I | R | A | I |

---

## Descripción del Flujo Completo

> **Sección nueva — no existía en el documento original.**
> **Justificación:** el flujo original solo era una lista numerada sin explicar cómo se conectan las decisiones y excepciones entre sí. Se describe aquí el recorrido completo en texto para que cualquier lector entienda el proceso de principio a fin, incluyendo las bifurcaciones que agregan las secciones anteriores (Fail the Build, excepciones, re-escaneo).

El proceso comienza cuando un docente o estudiante **solicita una imagen** para un curso o proyecto. El sistema realiza primero una **búsqueda automática en Harbor**: si la imagen ya existe y está vigente, se entrega directamente para su descarga, sin pasos adicionales.

Si la imagen **no existe**, la solicitud pasa al Responsable de Imágenes, quien la **revisa y aprueba** su creación. Una vez aprobada, la imagen se somete a un **escaneo de vulnerabilidades con Trivy**.

En este punto el flujo se bifurca según el resultado del escaneo:

- Si **no se detectan vulnerabilidades críticas o altas**, la imagen continúa directamente hacia la firma digital.
- Si **se detecta una vulnerabilidad crítica o alta**, se activa la política de **"Fail the Build"**: la publicación se bloquea automáticamente. Solo puede continuar si el **Chapter Lead de Seguridad aprueba una excepción documentada** (motivo, responsable y fecha límite de remediación). Sin esa excepción, la imagen queda rechazada y no se publica.

Una vez que la imagen pasa el escaneo (o cuenta con la excepción aprobada), se **firma digitalmente con Cosign/Sigstore** y se **publica en Harbor junto con sus metadatos de trazabilidad**.

A partir de la publicación, el estudiante puede **descargar la imagen oficial**, y el script de descarga **verifica automáticamente la firma** antes de permitir su ejecución, tanto en el laboratorio como en su computadora personal.

Finalmente, el ciclo no termina en la publicación: cada mes se ejecuta un **re-escaneo automático de todas las imágenes activas**. Si ese re-escaneo detecta una vulnerabilidad nueva en una imagen ya publicada, se notifica al Responsable de Imágenes y se vuelve a aplicar la política de "Fail the Build", generándose una nueva versión corregida bajo un tag inmutable, sin sobrescribir la anterior, para no romper la reproducibilidad de prácticas ya evaluadas con esa versión.
