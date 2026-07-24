# Informe de Revisión y Comentarios
## Documento 1 — Auditoría de la Propuesta del Repositorio

**Asignatura:** Organización y Métodos  
**Universidad:** Universidad Nacional de San Agustín de Arequipa  
**Equipo consultor:** Equipo A  
**Año:** 2026

---

## 1. Introducción

El presente informe recoge los comentarios de auditoría elaborados por los cuatro integrantes del equipo consultor sobre la propuesta del repositorio «Plataforma Híbrida de Gestión de Laboratorios de Computación». Cada integrante evaluó los documentos asignados actuando como consultor de Organización y Métodos (O&M), respondiendo las siguientes preguntas para cada archivo: qué aspectos están correctamente desarrollados, qué elementos pueden mejorarse, qué información falta y qué acciones se proponen.

El objetivo de este informe es identificar las brechas entre la propuesta actual y las buenas prácticas de O&M, BPMN 2.0, ITIL 4, ISO 9001:2015, ISO/IEC 27001:2022, COBIT 2019 y DevSecOps, para así fundamentar las propuestas de mejora del Documento 2.

---

## 2. Metodología de revisión

### 2.1 Criterios utilizados

La revisión se realizó aplicando los siguientes marcos de referencia y estándares:

- **BPMN 2.0** — Para evaluar la representación y completitud de los flujos de proceso.
- **ITIL 4** — Para verificar la existencia de un catálogo de servicios, SLAs y gestión de incidentes.
- **ISO 9001:2015** — Para revisar la definición de indicadores, responsables y criterios de aceptación.
- **ISO/IEC 27001:2022** — Para evaluar controles de seguridad, gestión de accesos y políticas de seguridad de imágenes.
- **COBIT 2019** — Para analizar la gobernanza de TI, la gestión del riesgo y la continuidad del servicio.
- **DevSecOps / Docker Security Benchmark** — Para revisar el ciclo de vida de imágenes de contenedores, escaneo de vulnerabilidades y firma digital.

### 2.2 Alcance de la auditoría

Los archivos revisados por cada integrante fueron los siguientes:

| Integrante | Archivos auditados |
|---|---|
| Paola Adamari Mayta Quispe | `README.md`, `README2.MD` |
| Romina Giuliana Camargo Hilachoque | `docs/arquitectura.md`, `docs/fases-implementacion.md`, `docs/gestion-imagenes (1).md` |
| José León Enrique Hatches Curo | `docs/procesos-laboratorio.md`, `docs/procesos/procesos-laboratorio.md`, `docs/procesos/procesos-laboratorio02.md`, `docs/procesos/procesos-laboratorio03.md`, `docs/procesos/procesos-laboratorio04.md` |
| José Manuel Morocco Saico | `docs/organizacion-agil.md`, `docs/plan-dedicacion.md`, `backlog/inicial.md`, Matriz RACI en `docs/procesos-laboratorio.md` |

---

## 3. Comentarios del Integrante 1 — Paola Adamari Mayta Quispe

### 3.1 `README.md`

#### ¿Qué está bien?

- El archivo presenta claramente la problemática relacionada con la gestión fragmentada de los laboratorios de computación.
- Los objetivos propuestos guardan relación con las necesidades identificadas: estandarización de entornos, trazabilidad del software, administración de usuarios y gestión de recursos físicos.
- Ofrece una visión general de la arquitectura, las fases de implementación y el modelo organizacional del proyecto.
- Considera beneficios tanto para el ámbito universitario como para una futura aplicación empresarial.

#### ¿Qué está mal o puede mejorarse?

- El documento mezcla las necesidades universitarias y empresariales sin delimitar claramente las características correspondientes a cada versión de la plataforma.
- Los objetivos y beneficios están expresados de manera general, sin indicadores, valores iniciales ni metas que permitan comprobar su cumplimiento.
- Se propone utilizar el modelo Spotify sin justificar suficientemente si resulta viable para la cantidad real de integrantes disponibles.
- Se observan problemas de codificación de caracteres y referencias a documentos que actualmente no existen en el repositorio.

#### ¿Qué falta?

- Falta identificar formalmente a la universidad, los responsables del proyecto, las partes interesadas y la población beneficiaria.
- No se define el alcance, las exclusiones, los supuestos, las restricciones, los riesgos ni el presupuesto estimado.
- Se requieren indicadores de éxito: reducción del tiempo de instalación, disponibilidad de la plataforma y nivel de satisfacción de los usuarios.
- Faltan documentos mencionados en el propio README: `roles-habilidades.md`, `costos.md`, `CODE_OF_CONDUCT.md` y `CONTRIBUTING.md`.
- Se necesita desarrollar la gobernanza del software, los datos, las licencias y las imágenes Docker.

#### ¿Qué proponemos?

- Separar claramente la versión académica de la empresarial mediante una tabla que indique funcionalidades, entregables y criterios de aceptación de cada una.
- Convertir los objetivos en metas SMART, con indicadores, responsables y medios de verificación.
- Corregir la codificación de caracteres y eliminar o completar las referencias a documentos inexistentes.
- Incorporar secciones sobre alcance, interesados, riesgos, presupuesto y gobernanza.
- Conservar el README como una presentación ejecutiva y dirigir mediante enlaces a la documentación detallada en la carpeta `docs`.

---

### 3.2 `README2.MD`

#### ¿Qué está bien?

- Funciona como un resumen de la propuesta principal y permite reconocer rápidamente el problema, los objetivos y los beneficios del proyecto.
- Su estructura breve facilita que los interesados comprendan la idea antes de consultar la documentación detallada.
- Incluye enlaces hacia los documentos relacionados con la organización ágil, la arquitectura, la gestión de imágenes y las fases de implementación.

#### ¿Qué está mal o puede mejorarse?

- Repite gran parte de la información contenida en `README.md`, lo cual puede provocar contradicciones si uno de los dos archivos se actualiza y el otro no.
- La tabla de contenidos combina enlaces internos y externos de manera inconsistente.
- No explica cuál es el alcance mínimo viable, quiénes son los principales usuarios ni cuál es el avance real del proyecto.
- Algunos enlaces están rotos, como el correspondiente a `docs/gestion-imagenes.md`, debido a que dicho archivo ya no existe con ese nombre en la versión actual del repositorio.

#### ¿Qué falta?

- Falta indicar que este archivo es un resumen ejecutivo y especificar cuál de los dos README constituye la fuente oficial del proyecto.
- Deben incluirse los responsables, la fecha de la última actualización, los próximos hitos, los principales riesgos y algunos indicadores resumidos de éxito.
- Se necesita diferenciar la versión académica de la empresarial y corregir las referencias hacia archivos inexistentes, como `docs/roles-habilidades.md`.

#### ¿Qué proponemos?

- Utilizar `README.md` como la portada y fuente principal del proyecto.
- Convertir `README2.MD` explícitamente en un resumen ejecutivo o eliminarlo para evitar la duplicación de información.
- Si se conserva, incluir una tabla breve con el alcance, los beneficiarios, los entregables, los responsables y el estado del proyecto.
- Corregir la codificación de caracteres, actualizar los enlaces y establecer una revisión periódica que permita detectar referencias rotas antes de cada entrega.

---

## 4. Comentarios del Integrante 2 — Romina Giuliana Camargo Hilachoque

### 4.1 `docs/arquitectura.md`

#### ¿Qué está bien?

- El modelo híbrido On-Premise + Nube es acertado: aprovecha la infraestructura local para las cargas recurrentes de clase y reserva la nube para picos de demanda.
- El stack es íntegramente open source (GitLab, Harbor, Keycloak, Kubernetes, PostgreSQL, MinIO), lo cual es conveniente para una institución con presupuesto limitado.
- Keycloak centraliza la identidad de estudiantes y docentes en un solo directorio, algo clave dada la alta rotación semestral de usuarios.
- El principio de "entorno idéntico dentro y fuera del laboratorio" resuelve el problema pedagógico de que el estudiante practique en casa con una configuración distinta a la del aula.

#### ¿Qué está mal o puede mejorarse?

- No se explica cómo Kubernetes soportará el "efecto campana": toda un aula iniciando su entorno al mismo tiempo al comenzar la clase.
- No se define un modelo de alta disponibilidad ni un plan de contingencia si Proxmox falla durante una clase en curso.
- No hay segmentación de red entre el segmento estudiantil y el segmento de gestión (Harbor, GitLab, Keycloak).
- No se indica si los recursos estarán segmentados por curso o carrera, lo que puede hacer que un curso intensivo degrade a otros.

#### ¿Qué falta?

- Ausencia de políticas de respaldo y recuperación ante desastres (DRP/BCP) para PostgreSQL, MinIO y Harbor.
- No hay SLOs orientados al contexto académico (ej. tiempo de aprovisionamiento por sesión de laboratorio).
- Falta un apartado de gestión de capacidad que proyecte cuántos estudiantes/cursos concurrentes soporta la arquitectura.
- No existe un catálogo de servicios (ITIL) que un docente sin perfil técnico pueda entender y usar.
- Falta observabilidad: no hay monitoreo ni alertas ante caídas de servicio.

#### ¿Qué proponemos?

- Probar el "efecto campana" con pruebas de carga y dimensionar Kubernetes/Proxmox en base a ese escenario.
- Definir SLOs académicos (ej. 99% de disponibilidad en horario lectivo) e implementar Prometheus + Grafana desde la Fase 0.
- Segmentar la red en zona "estudiante" y zona "plataforma" (GitLab, Harbor, Keycloak).
- Establecer cuotas de recursos por curso/carrera en Kubernetes.
- Incluir un respaldo 3-2-1 para MinIO/PostgreSQL, dado que ahí residirán entregables evaluables.

---

### 4.2 `docs/fases-implementacion.md`

#### ¿Qué está bien?

- La secuencia de fases (Diseño → Universidad → Empresa → Piloto → Mejora Continua) valida primero en un entorno académico controlado antes de escalar a uno empresarial.
- La Fase 4 de Mejora Continua reconoce que la plataforma evolucionará semestre a semestre junto con el currículo.
- Separar el Proyecto Universitario del Proyecto Empresa es coherente con el modelo formativo descrito en el README.

#### ¿Qué está mal o puede mejorarse?

- Las fases solo tienen nombre y duración, sin entregables ni criterios de aceptación evaluables por fase.
- No se aclara cómo las duraciones (4-6, 5-7 meses) se alinean con el calendario semestral, lo que puede interrumpir trabajo a mitad de ciclo.
- No hay continuidad definida cuando la cohorte que ejecutó la Fase 1 se gradúa antes de iniciar la Fase 2.
- No se contempla capacitación previa de los docentes que liderarán Chapters, rol exigido por el README.

#### ¿Qué falta?

- No hay hitos de control (gates) ni criterios de salida medibles entre fases.
- Falta una matriz de riesgos propia del entorno universitario (rotación de estudiantes, disponibilidad docente, periodos de examen).
- No se define un plan de rollback si el Piloto (Fase 3) afecta una clase en curso.
- No hay un Product Owner institucional que dé continuidad entre cohortes.
- Falta referencia a presupuesto y a transferencia de conocimiento entre generaciones de estudiantes.

#### ¿Qué proponemos?

- Alinear cada fase al calendario académico (ej. Fase 1 = 2 semestres consecutivos).
- Definir criterios de salida medibles (ej. "3 cursos usando la plataforma sin incidentes críticos") en vez de basarse solo en tiempo.
- Crear un plan de transferencia de conocimiento entre cohortes (documentación viva, wiki del proyecto).
- Nombrar un Product Owner institucional permanente que no rote con cada cohorte.
- Añadir una matriz de riesgos académica y un plan de rollback para el Piloto.

---

### 4.3 `docs/gestion-imagenes (1).md`

#### ¿Qué está bien?

- El escaneo con Trivy y la firma de imagen antes de publicar son buenas prácticas DevSecOps, con valor formativo adicional para los estudiantes.
- La aprobación humana antes de crear una imagen evita que cada curso genere la suya sin control.
- La búsqueda automática en Harbor promueve reutilización y evita entornos distintos entre secciones de un mismo curso.
- El beneficio de "mismo entorno dentro y fuera del laboratorio" resuelve directamente el problema de instalaciones manuales descrito en el README.

#### ¿Qué está mal o puede mejorarse?

- No se define qué pasa si Trivy detecta una vulnerabilidad crítica en una imagen urgente para la clase de esa semana.
- No hay SLA de aprobación para la revisión manual, riesgoso si un docente necesita una imagen días antes de una práctica.
- No se especifica cómo se verifica la firma en las computadoras personales de los estudiantes, fuera del control del laboratorio.
- No se contempla la actualización de una imagen ya publicada, solo su creación inicial.

#### ¿Qué falta?

- No hay política de versionado (tags inmutables por semestre vs. `latest`), clave para reproducibilidad de prácticas evaluadas.
- Falta una política de retención de imágenes de semestres anteriores.
- No hay proceso de re-escaneo periódico de imágenes ya publicadas.
- No se define un SLA operativo del flujo completo.
- Falta una matriz RACI que aclare si "el Responsable" es el docente, el equipo de plataforma o el Chapter Lead de seguridad.

#### ¿Qué proponemos?

- Implementar una política de "fail the build" con excepción única documentada por el Chapter Lead de seguridad para urgencias.
- Establecer un SLA de aprobación (ej. 5 días hábiles) y exigir solicitudes con al menos 2 semanas de anticipación a la práctica.
- Adoptar Cosign/Sigstore e incluir la verificación de firma en el script de descarga del estudiante.
- Aplicar versionado inmutable por semestre (ej. `curso-bd:2026-1`) y retención de solo las últimas 3 versiones.
- Ejecutar un re-escaneo mensual de imágenes activas y crear una matriz RACI que separe aprobación de curso (docente) y de seguridad (Chapter Lead).

---

## 5. Comentarios del Integrante 3 — José León Enrique Hatches Curo

### 5.1 `docs/procesos-laboratorio.md`

#### ¿Qué está bien?

- Identifica correctamente a los actores clave (Administrador de laboratorio, Responsable de Imágenes, Docente, Estudiante) y cuenta con una matriz RACI.
- Integra el concepto de "Chapter de Organización" para mantener la mejora continua sin entorpecer a los equipos técnicos.
- Propone un set inicial de KPIs, lo cual es excelente para la medición del desempeño.

#### ¿Qué está mal o puede mejorarse?

- La representación de los procesos BPMN es exclusivamente textual, por lo que no cumple con el estándar visual formal para el modelado de procesos.
- La matriz RACI asigna el rol de "R/A" (Responsable y Aprobador) al Responsable de Imágenes en la creación de nuevas imágenes, rompiendo el principio de segregación de funciones.

#### ¿Qué falta?

- Faltan los diagramas BPMN reales elaborados en herramientas gráficas.
- Falta incluir flujos de procesos de soporte críticos sugeridos en el mismo documento: Gestión de Incidentes y Onboarding de Nuevos Usuarios.

#### ¿Qué proponemos?

- Rediseñar la Matriz RACI separando claramente quién ejecuta (R) y quién aprueba (A).
- Elaborar fichas técnicas detalladas para los KPIs propuestos.
- Modelar gráficamente todos los procesos bajo el estándar BPMN 2.0.

---

### 5.2 `docs/procesos/procesos-laboratorio.md`

#### ¿Qué está bien?

- Define un objetivo claro: estandarizar el funcionamiento, reducir tiempos improductivos y garantizar la trazabilidad.
- Menciona el uso de diagramas BPMN para representar flujos, roles, actividades y decisiones de forma clara.

#### ¿Qué está mal o puede mejorarse?

- La tabla de "Roles Principales (RACI)" es únicamente descriptiva y no realiza el cruce matricial real de responsabilidades.
- El documento está incompleto y se corta en el título "3.1 Proceso 1: Solicitud y Asignación de Recursos (Hardware)", sugiriendo que es una versión obsoleta.

#### ¿Qué falta?

- Falta el desarrollo de los procesos y los diagramas prometidos en la introducción.

#### ¿Qué proponemos?

- Construir tablas formales de actividades, entradas y salidas para cada proceso.
- Completar el documento integrando los diagramas BPMN 2.0 definitivos.

---

### 5.3 `docs/procesos/procesos-laboratorio02.md`

#### ¿Qué está bien?

- Contempla pasos de seguridad fundamentales, incluyendo un escaneo de vulnerabilidades y una aprobación antes de publicar la imagen.
- Separa la lógica entre encontrar una imagen oficial existente y tener que crear una imagen personalizada.

#### ¿Qué está mal o puede mejorarse?

- La representación es solo texto en lugar de un diagrama formal.

#### ¿Qué falta?

- Falta un camino de rechazo para el "Escaneo de Seguridad", asumiendo que siempre será exitoso y pasará a la aprobación.
- Falta la definición de "Pools" y "Lanes" para los actores involucrados.

#### ¿Qué proponemos?

- Modelar el proceso de forma gráfica bajo el estándar BPMN 2.0.
- Diseñar el flujo visual utilizando carriles separados para el Docente/Estudiante, el Sistema y el Responsable de Imágenes.
- Agregar compuertas lógicas (XOR) para manejar los fallos en el escaneo de seguridad.

---

### 5.4 `docs/procesos/procesos-laboratorio03.md`

#### ¿Qué está bien?

- Utiliza herramientas de automatización como Renovate/Dependabot como evento de inicio del proceso.
- Realiza una distinción eficiente entre actualizaciones con cambios críticos (requieren intervención humana) y no críticos (actualización automática).

#### ¿Qué está mal o puede mejorarse?

- La representación es solo texto en lugar de un diagrama formal.
- La ruta de aprobación manual no contempla qué sucede si el responsable decide rechazar la actualización.

#### ¿Qué falta?

- Falta un evento de fin negativo en caso de que la actualización crítica sea rechazada o abortada.

#### ¿Qué proponemos?

- Modelar el proceso de forma gráfica bajo el estándar BPMN 2.0.
- Incorporar una compuerta lógica después del bloque de aprobación manual para gestionar el flujo de rechazo.

---

### 5.5 `docs/procesos/procesos-laboratorio04.md`

#### ¿Qué está bien?

- Cubre todo el ciclo de uso e implementa un mecanismo de control físico mediante un Check-in con Código QR.

#### ¿Qué está mal o puede mejorarse?

- La representación es solo texto en lugar de un diagrama formal.
- La ruta alternativa cuando no hay equipos disponibles finaliza en un callejón sin salida ("Ver Alternativas o Esperar") sin ofrecer una resolución sistémica clara.

#### ¿Qué falta?

- Falta un manejo de excepciones de tiempo: definir qué ocurre si el usuario reserva pero no realiza el Check-in.

#### ¿Qué proponemos?

- Modelar el proceso de forma gráfica bajo el estándar BPMN 2.0.
- Añadir un evento intermedio de tiempo ("Timer Event") en el BPMN que libere el equipo automáticamente si no se registra el Check-in en un tiempo prudencial.

