# Documento 2 — Propuesta de Organización

**Asignatura:** Organización y Métodos  
**Universidad:** Universidad Nacional de San Agustín de Arequipa  
**Equipo consultor:** Equipo A  
**Año:** 2026

> Documento colaborativo. Cada integrante incorporará las secciones correspondientes a su rol.

## 1. Introducción

**Responsable:** Paola Adamari Mayta Quispe — Scrum Master

La gestión eficiente de los laboratorios de computación constituye un elemento importante para el desarrollo de las actividades académicas, debido a que estos espacios concentran infraestructura tecnológica, aplicaciones, cuentas de usuario y entornos de trabajo utilizados por docentes y estudiantes. Sin embargo, cuando su administración se realiza mediante procedimientos manuales o poco estandarizados, pueden presentarse problemas como duplicidad de reservas, demora en la instalación de software, diferencias entre los entornos de trabajo y falta de trazabilidad sobre los recursos utilizados.

A partir de la revisión del repositorio «Plataforma Híbrida de Gestión de Laboratorios de Computación», el equipo consultor identificó fortalezas relacionadas con la estandarización de entornos, el uso de imágenes Docker y la integración de herramientas tecnológicas. También se encontraron oportunidades de mejora en la definición de responsabilidades, documentación de procesos, gestión de incidencias, control de licencias, seguridad y continuidad operativa.

Por esta razón, el presente documento propone una estructura organizacional para la gestión del laboratorio. La propuesta define actores, responsabilidades, mecanismos de comunicación y escalamiento, procesos organizacionales, indicadores de desempeño y lineamientos para la gobernanza de imágenes Docker, software y licencias.

El propósito es establecer un modelo de gestión ordenado, seguro, trazable y adaptable a las necesidades académicas, que permita aprovechar adecuadamente los recursos del laboratorio y facilite una futura evolución hacia un entorno empresarial.

## 2. Metodología de la consultoría

**Responsable:** Paola Adamari Mayta Quispe — Scrum Master

La consultoría se desarrolló mediante un enfoque de revisión documental y mejora de procesos. Como fuente principal se utilizó el repositorio proporcionado por el docente, compuesto por los archivos README, el backlog y la documentación ubicada en la carpeta `docs`.

El trabajo se inició con la distribución de los archivos entre los cuatro integrantes. Cada miembro evaluó los documentos asignados considerando cuatro preguntas: qué aspectos estaban correctamente desarrollados, qué elementos podían mejorarse, qué información faltaba y qué acciones se proponían.

Posteriormente, los hallazgos individuales fueron reunidos para elaborar un diagnóstico de la situación actual o AS-IS. Este diagnóstico sirvió como base para construir la propuesta de situación futura o TO-BE, conformada por una estructura organizacional, roles, matrices de responsabilidad, procesos, indicadores y mecanismos de gobernanza.

Finalmente, el equipo revisó la coherencia entre los problemas identificados y las soluciones propuestas. Las actividades fueron coordinadas mediante principios de Scrum y un tablero Kanban simplificado para controlar el avance y la revisión de los entregables.

### 2.1 Organización del equipo consultor

Para desarrollar la consultoría se asignaron roles que permitieron distribuir las responsabilidades de acuerdo con los componentes principales del trabajo.

| Integrante | Rol | Responsabilidad principal |
|---|---|---|
| Paola Adamari Mayta Quispe | Scrum Master | Coordinar las actividades, organizar el cronograma y el tablero Kanban, redactar la metodología, revisar la coherencia del documento y elaborar las recomendaciones y conclusiones finales. |
| Romina Giuliana Camargo Hilachoque | Product Owner | Elaborar el diagnóstico AS-IS, definir la propuesta TO-BE y comprobar que las mejoras respondan a las necesidades del laboratorio. |
| José León Enrique Hatches Curo | Analista BPMN | Diseñar y documentar los procesos, identificando actividades, responsables, entradas, salidas y decisiones. |
| José Manuel Morocco Saico | Analista Organizacional | Definir la estructura organizacional, los roles, la matriz RACI, los mecanismos de comunicación, el escalamiento, los indicadores y la gobernanza. |

Aunque cada integrante asumió una responsabilidad principal, la revisión final se realizó de manera conjunta para evitar contradicciones entre los procesos, roles y recomendaciones.

### 2.2 Metodología aplicada

La metodología se organizó en seis etapas:

#### Etapa 1: Revisión y levantamiento de información

Se revisaron los archivos del repositorio para comprender el propósito de la plataforma, sus objetivos, componentes técnicos, procesos y modelo organizacional.

#### Etapa 2: Auditoría documental

Cada integrante evaluó los archivos asignados empleando criterios relacionados con claridad, coherencia, viabilidad, trazabilidad, seguridad y gestión de procesos. Los resultados fueron registrados como comentarios dentro del repositorio y en el Informe de Revisión.

#### Etapa 3: Diagnóstico AS-IS

Los hallazgos fueron consolidados para describir la situación actual. Se identificaron problemas como falta de responsables claramente definidos, procesos incompletos, ausencia de indicadores, riesgos de seguridad y debilidades en el control del software y las licencias.

#### Etapa 4: Diseño de la propuesta TO-BE

Sobre la base del diagnóstico se definió una estructura organizacional mejorada, acompañada de roles, responsabilidades, matrices organizacionales y procesos BPMN.

#### Etapa 5: Validación y revisión

Se verificó que cada problema identificado tuviera una recomendación o mecanismo de solución. También se revisó la coherencia entre la matriz RACI, los procesos, los indicadores y la estructura organizacional.

#### Etapa 6: Consolidación de entregables

Finalmente, se integraron los aportes en dos productos: el Informe de Revisión y Comentarios y la Propuesta de Organización.

### 2.3 Cronograma y recursos de la consultoría

El trabajo documental se organizó en cuatro jornadas. Esta planificación representa el esfuerzo del equipo consultor y no el tiempo de implementación técnica de toda la plataforma.

| Actividad | Responsable principal | Duración | Esfuerzo estimado | Recurso requerido | Resultado |
|---|---|---:|---:|---|---|
| Revisión del repositorio | Todo el equipo | 1 día | 2 h por integrante | Repositorio y documentos base | Comprensión de la propuesta |
| Distribución de archivos | Scrum Master | 1 día | 1 h | Reunión de coordinación | Responsabilidades asignadas |
| Auditoría documental | Todos, según asignación | 2 días | 4 h por integrante | GitHub y criterios de revisión | Comentarios por archivo |
| Diagnóstico AS-IS | Product Owner | 1 día | 4 h | Hallazgos de la auditoría | Problemas identificados |
| Diseño de procesos | Analista BPMN | 2 días | 6 h | Herramienta de modelado | Procesos documentados |
| Diseño organizacional | Analista Organizacional | 2 días | 6 h | Matrices y documentación | Roles, matrices y gobierno |
| Revisión integral | Scrum Master y equipo | 1 día | 2 h por integrante | Documento consolidado | Corrección de inconsistencias |
| Consolidación y presentación | Todo el equipo | 1 día | 2 h por integrante | Word, Markdown y GitHub | Entregables finales |

El plan detallado para ejecutar la propuesta, incluyendo calendario académico, capacidad del equipo y costos, se desarrolla en la sección 10.

### 2.4 Tablero Kanban resumido

| Pendiente | En proceso | En revisión | Terminado |
|---|---|---|---|
| Ajustes derivados de la exposición | Validación final de formato | Coherencia entre procesos y RACI | Revisión del repositorio |
| Cotización institucional del piloto | Estimación detallada de recursos | Revisión ortográfica | Auditoría de archivos |
| Validación del roadmap |  |  | Diagnóstico AS-IS |
|  |  |  | Propuesta TO-BE |
|  |  |  | Procesos y matrices |

El Scrum Master actualiza el tablero después de cada reunión. Una actividad solo pasa a “Terminado” cuando cuenta con evidencia, responsable identificado y revisión de al menos otro integrante.
---

## 3. Diagnóstico organizacional (AS-IS)

La gestión de los laboratorios de cómputo tradicionales en la institución presenta ineficiencias estructurales críticas bajo el enfoque de procesos de Organización y Métodos (O&M). Al evaluar el flujo de valor, se evidencia que el modelo tradicional es incompatible con la agilidad que exige nuestro calendario académico.

![diagrama de árbol de problemas: Instalación Manual vs. Falta de Auditoría](./architecture/grafico1.jpg)
Para dimensionar el impacto de estos problemas en la realidad académica de la facultad, se ha elaborado la siguiente matriz de diagnóstico:
## 10. Plan de implementación y viabilidad de recursos

**Responsable:** Paola Adamari Mayta Quispe — Scrum Master

Con base en la auditoría realizada en el Documento 1, se identificaron riesgos críticos para la viabilidad del proyecto original: duraciones que no se alinean con el calendario académico, cargas horarias insostenibles para los estudiantes y ausencia de una estimación de costos de infraestructura, red y contingencia.

Para convertir la propuesta organizacional en un proyecto ejecutable, el presente plan integra tres instrumentos: un roadmap vinculado al calendario académico, un cálculo de capacidad sostenible del equipo y una matriz referencial de inversión tecnológica. Estos instrumentos deberán revisarse al inicio de cada semestre con información real de matrícula, inventario, disponibilidad docente y cotizaciones.

### Principios de viabilidad

- No iniciar una fase sin aprobar los entregables y recursos de la fase anterior.
- Reutilizar infraestructura existente cuando cumpla los requisitos de capacidad y seguridad.
- Ajustar el alcance del sprint a la disponibilidad académica real de los estudiantes.
- Ejecutar primero un piloto controlado antes de comprometer un escalamiento institucional.
- Tratar los costos como estimaciones sujetas a inventario, cotización y aprobación institucional.

### 10.1 Roadmap de implementación académica

El roadmap corrige la equivalencia temporal del proyecto original y organiza el trabajo alrededor de un año lectivo estándar de dos semestres de 17 semanas. La validación del MVP durante el periodo intersemestral estará condicionada a la disponibilidad voluntaria o formalmente asignada del equipo.

| Fase | Nombre | Duración | Ancla académica | Hito de salida |
|---:|---|---:|---|---|
| 0 | Diagnóstico y diseño detallado | 4 semanas | Semanas 1–4 del semestre 1 | Arquitectura, alcance e inventario de hardware aprobados. |
| 1A | MVP académico: construcción | 12 semanas | Semanas 5–16 del semestre 1 | Plataforma desplegada con infraestructura base operativa. |
| 1B | MVP académico: validación | 4 semanas | Semana 17 e intersemestre | KPIs evaluados, documentación revisada y controles de seguridad ejecutados con Trivy. |
| 2 | Piloto controlado de 1 a 3 cursos | 8 semanas | Semanas 5–12 del semestre 2 | Sin interrupciones críticas no mitigadas y satisfacción de usuarios igual o superior al 85 %. |
| 3 | Evaluación y estabilización | 4 semanas | Semanas 13–16 del semestre 2 | Informe de cierre, costos reales y lecciones aprendidas aprobados. |
| 4 | Escalamiento institucional | 12 semanas o más | Semestre 3 en adelante | Aprobación formal para ampliar la plataforma a la facultad. |

Cada fase funciona como una puerta de decisión. Si no se cumple el hito de salida, el comité de gobierno deberá corregir el alcance, ampliar el plazo o suspender temporalmente el avance, en lugar de trasladar riesgos abiertos a la fase siguiente.

### 10.2 Planificación de capacidad y horas sostenibles

Para evitar sobrecarga y mantener un ritmo sostenible, se descarta la dedicación original de 25 horas semanales por estudiante. El Product Owner debe ajustar el sprint backlog a la capacidad disponible en cada periodo:

| Periodo académico | Capacidad por estudiante | Criterio de planificación |
|---|---:|---|
| Semana regular sin cruces críticos | 10–12 h/semana | Desarrollo, revisión y documentación. |
| Semana de entregas parciales | 6–8 h/semana | Reducir alcance y priorizar entregables obligatorios. |
| Semana de exámenes finales | 0–3 h/semana | Sprint mínimo dedicado únicamente a mantenimiento crítico. |
| Vacaciones intersemestrales | 15–20 h/semana | Solo con disponibilidad confirmada; validación intensiva y documentación. |

La capacidad comprometida del equipo se calculará al inicio de cada sprint:

> **Capacidad del sprint = integrantes disponibles × horas disponibles × factor de enfoque**

Se recomienda utilizar inicialmente un factor de enfoque de 0,70, reservando el 30 % restante para reuniones, aprendizaje, incidencias y tareas no previstas. Si la capacidad disminuye por exámenes u otras asignaturas, se reducirá el alcance antes de aumentar las horas de trabajo.

### 10.3 Matriz referencial de costos e inversión tecnológica

GitLab, Harbor, Kubernetes y Keycloak disponen de ediciones de código abierto, pero su operación requiere infraestructura, energía, almacenamiento, respaldo y personal. La siguiente matriz presenta rangos preliminares en soles; no reemplaza el inventario institucional ni las cotizaciones de proveedores.

| N.º | Categoría | Componentes o supuesto mínimo | Tipo | Presupuesto referencial |
|---:|---|---|---|---:|
| 1 | Servidor principal | Servidor físico para Proxmox VE, mínimo 32 GB RAM y 8 núcleos | CAPEX | S/ 8 000–15 000 |
| 2 | Nodos de alta disponibilidad | Servidores adicionales para Kubernetes; cantidad definida por la prueba de capacidad | CAPEX | S/ 5 000–10 000 por nodo |
| 3 | Almacenamiento persistente | SSD/NVMe para Harbor y MinIO, mínimo 4 TB brutos antes de redundancia | CAPEX | S/ 1 500–3 000 |
| 4 | Equipamiento de red | Switch administrable con VLAN para zonas de estudiantes, plataforma y datos | CAPEX | S/ 800–2 000 |
| 5 | Servicios de nube | Instancias para respaldo, contingencia o picos de demanda | OPEX | S/ 500–1 500 al mes |
| 6 | Continuidad operativa | Electricidad, UPS, mantenimiento y reposición programada | OPEX | S/ 200–500 al mes |
| 7 | Contingencia técnica | Repuestos e imprevistos sobre la inversión aprobada | Reserva | 15 % del subtotal CAPEX |
| 8 | Licencias de software | MATLAB, IDE comerciales u otras herramientas solicitadas por docentes | CAPEX/OPEX | Sujeto al inventario y convenios universitarios |

Los rangos no deben sumarse automáticamente: el escenario final depende de la infraestructura reutilizable, el número de nodos, los meses de servicio en nube y las licencias ya cubiertas por convenios institucionales.

### 10.4 Control de viabilidad y aprobación presupuestaria

Antes de autorizar una adquisición o avanzar hacia el escalamiento, el comité de gobierno deberá revisar como mínimo:

| Control | Evidencia requerida | Responsable | Aprobador |
|---|---|---|---|
| Inventario reutilizable | Relación de servidores, red, almacenamiento y licencias disponibles | Administrador de Plataforma | Encargado de Laboratorio |
| Dimensionamiento | Prueba de carga con usuarios concurrentes y consumo medido | Equipo técnico | Comité de Gobierno |
| Comparación económica | Al menos tres cotizaciones o precios públicos comparables | Encargado de Laboratorio | Dirección / Comité de TI |
| Costo total de propiedad | CAPEX, OPEX, mantenimiento, energía y renovación a tres años | Product Owner | Dirección / Comité de TI |
| Disponibilidad del equipo | Horas asignadas de docentes, estudiantes y soporte | Scrum Master | Product Owner |
| Resultado del piloto | KPIs, incidentes, satisfacción, costos reales y lecciones aprendidas | Equipo consultor | Comité de Gobierno |

Las estimaciones deberán actualizarse cuando una cotización tenga más de 90 días, cambie el alcance o la prueba de capacidad muestre una variación superior al 20 %. El escalamiento solo será viable si cuenta con presupuesto aprobado, personal operativo asignado y cumplimiento de los criterios de salida del piloto.

## 11. Recomendaciones de implementación

**Responsable:** Paola Adamari Mayta Quispe — Scrum Master

Se recomienda implementar la propuesta de manera progresiva, comenzando con un piloto controlado en un laboratorio y un número reducido de cursos. Antes de incorporar la plataforma, deberán aprobarse formalmente los roles, responsabilidades, presupuesto y procesos operativos.

Asimismo, se recomienda:

1. Designar un responsable institucional permanente que garantice la continuidad del proyecto entre distintos semestres.
2. Formalizar la matriz RACI y comunicarla a docentes, estudiantes, administradores y personal de soporte.
3. Implementar inicialmente los procesos prioritarios: solicitud de imágenes, reserva de laboratorios, gestión de incidencias y administración de usuarios.
4. Establecer acuerdos de nivel de servicio para solicitudes, incidentes y disponibilidad de la plataforma.
5. Crear una política de gobernanza de imágenes Docker, software y licencias.
6. Mantener un inventario actualizado de hardware, software, cuentas, imágenes y licencias.
7. Capacitar a docentes, estudiantes y personal técnico antes del inicio del piloto.
8. Aplicar controles de seguridad como acceso por roles, escaneo de vulnerabilidades, firma de imágenes y registro de auditoría.
9. Medir indicadores como disponibilidad, utilización del laboratorio, tiempo de atención, satisfacción de usuarios y cantidad de incidentes.
10. Realizar revisiones periódicas para actualizar los procesos, riesgos y documentos.
11. Implementar respaldos y pruebas de recuperación para garantizar la continuidad operativa.
12. Validar los costos mediante inventario y cotizaciones antes de comprometer adquisiciones.
13. Ampliar la plataforma a otros laboratorios únicamente después de verificar los resultados técnicos, económicos y organizacionales del piloto.

## 12. Conclusiones

**Responsable:** Paola Adamari Mayta Quispe — Scrum Master

La revisión permitió determinar que la propuesta original constituye una base tecnológica útil para modernizar la gestión de los laboratorios de computación. Sus principales fortalezas son la estandarización de entornos, la utilización de imágenes de contenedores, la trazabilidad del software y la posibilidad de integrar recursos locales y servicios en la nube.

Sin embargo, la tecnología por sí sola no garantiza una gestión eficiente. Para que la plataforma funcione correctamente es necesario complementarla con una estructura organizacional, responsables definidos, procesos formalizados, canales de comunicación, mecanismos de escalamiento e indicadores de desempeño.

La propuesta desarrollada responde a estas necesidades mediante la definición de una situación futura o TO-BE. Esta considera la participación del director, encargado del laboratorio, administrador de la plataforma, docentes, estudiantes y personal de soporte, con responsabilidades diferenciadas.

El roadmap propuesto reconoce que la disponibilidad de tiempo, personal e infraestructura es limitada. Por ello, plantea validar el inventario y el presupuesto antes de iniciar adquisiciones, ejecutar un piloto reducido y condicionar el escalamiento a resultados medibles.

Finalmente, se concluye que la implementación debe realizarse gradualmente, evaluando sus resultados antes de ampliar el alcance. La mejora continua, la capacitación, la seguridad y la gobernanza del software serán factores indispensables para asegurar la sostenibilidad de la plataforma.
