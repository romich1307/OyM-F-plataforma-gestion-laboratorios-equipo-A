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
