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
**Responsable:** Romina Camargo Hilachoque — Product Owner

La gestión de los laboratorios de cómputo tradicionales en la institución presenta ineficiencias estructurales críticas bajo el enfoque de procesos de Organización y Métodos (O&M). Al evaluar el flujo de valor, se evidencia que el modelo tradicional es incompatible con la agilidad que exige nuestro calendario académico.

<div align="center">
  <img src="./architecture/grafico1.jpg" alt="diagrama de árbol de problemas: Instalación Manual vs. Falta de Auditoría" width="80%">
</div>
Para dimensionar el impacto de estos problemas en la realidad académica de la facultad, se ha elaborado la siguiente matriz de diagnóstico:

| Problema Identificado (AS-IS) | Descripción de la Deficiencia | Impacto Operativo y Académico |
| :--- | :--- | :--- |
| **Instalación Manual (Cuello de Botella)** | El equipo de soporte instala el software requerido máquina por máquina al inicio del ciclo. | Toma de 2 a 3 semanas. En un semestre de 16 semanas (agosto-diciembre), representa una pérdida de casi el 20% del tiempo lectivo. |
| **Inconsistencia de Entornos** | Falta de estandarización entre las computadoras del laboratorio y las PCs portátiles de los estudiantes. | Alta tasa de incidentes técnicos en clase ("Funciona en mi máquina") y pérdida de tiempo diagnosticando errores. |
| **Ausencia de SLAs Operativos** | Solicitudes de nuevo software mediante procesos burocráticos y manuales sin tiempos de respuesta definidos. | Los docentes pueden esperar semanas por una aplicación, retrasando o cancelando prácticas de laboratorio. |
| **Falta de Trazabilidad y Gobernanza** | Nulo control sobre versiones instaladas, procedencia del código y estado de las licencias de uso. | Riesgos legales por infracción de propiedad intelectual y exposición a brechas de seguridad informática. |
| **Subutilización de Hardware** | Reservas gestionadas por canales informales (correos o bases de datos desactualizadas). | Solapamiento de horarios, tiempos muertos entre clases y subutilización de la infraestructura instalada. |

---

## 4. Propuesta de estructura organizacional (TO-BE)
**Responsable:** Romina Camargo Hilachoque — Product Owner

Para resolver los cuellos de botella detectados en el AS-IS y garantizar que el proyecto mantenga continuidad entre los semestres académicos, se propone adoptar un **Modelo Organizacional Ágil (Spotify Adaptado)**. 

<div align="center">
  <img src="./architecture/grafico2.jpg" alt="diagrama de estructura organizacional: Tribu, Chapters y Squads" width="90%">
</div>

El equipo consultor ha definido que esta estructura no implica que los estudiantes actuales desarrollen la plataforma, sino que establece el marco de trabajo metodológico que deberá seguir el equipo técnico asignado para evitar el desorden. La propuesta se organiza de la siguiente manera:

| Nivel Estructural | Equipo / Rol | Misión Organizacional TO-BE |
| :--- | :--- | :--- |
| **Alineación Estratégica** | **Tribu: "Platform Lab"** | Liderada por el Director de Laboratorio (Product Owner General). Asegura la continuidad del proyecto entre semestres y alinea el trabajo técnico con los objetivos académicos. |
| **Ejecución (Vertical)** | **Squad Core Platform** | Asegura la estabilidad de la red, los servidores (Proxmox VE), el clúster de Kubernetes y el almacenamiento (MinIO). |
| **Ejecución (Vertical)** | **Squad Image & Container Mgt.** | Enfocado exclusivamente en construir, auditar, asegurar y firmar el catálogo de contenedores cumpliendo tiempos de entrega estrictos. |
| **Ejecución (Vertical)** | **Squad Hardware & Lab Ops.** | Gestiona el inventario físico, el control de accesos mediante códigos QR y el mantenimiento del hardware. |
| **Estandarización (Horizontal)** | **Chapters Técnicos** | Liderados por profesores con experiencia industrial. Garantizan la transferencia tecnológica y el uso de buenas prácticas de desarrollo. |
| **Auditoría (Transversal)** | **Chapter Organización y Métodos** | Asigna un Process Owner a cada squad para mapear flujos, auditar la Matriz RACI y simplificar la burocracia técnica. |

---

## 9. Gobernanza de Imágenes Docker, Software y Licencias
**Responsable:** Romina Camargo Hilachoque — Product Owner 

Como parte de la consultoría se identificó la necesidad de establecer una política formal de gobernanza para la administración de imágenes Docker, software y licencias.

### 9.1 ¿Qué es la gobernanza del software?
La gobernanza del software es el marco estructurado de directrices, políticas, procesos y controles organizacionales que regulan la adquisición, el desarrollo, el despliegue, el mantenimiento y el retiro de activos de software y contenedores dentro de una infraestructura tecnológica. Define con claridad los derechos de decisión, los roles y las responsabilidades, garantizando el cumplimiento técnico y legal del software utilizado.

### 9.2 ¿Por qué es necesaria?
En una plataforma híbrida de laboratorios basada en microservicios y contenedores, la gobernanza de TI es imprescindible para:
*   **Evitar la proliferación de contenedores no controlados (Registry Bloat):** Prevenir que se saturen los volúmenes de almacenamiento del registro privado (Harbor) con imágenes obsoletas, duplicadas o sin uso lectivo real.
*   **Garantizar la Seguridad del Entorno:** Asegurar que ninguna imagen contenga malware o dependencias con vulnerabilidades críticas conocidas que pongan en riesgo la red de la universidad o de la empresa cliente.
*   **Alineación de Cumplimiento Legal:** Mitigar riesgos de propiedad intelectual y demandas legales controlando estrictamente las licencias del software embebido en los contenedores.

### 9.3 y 9.4 Lineamientos de Gobernanza (Docker y Licencias)
Se establecen directrices obligatorias para regir el ciclo de vida de los contenedores y el control exhaustivo de la propiedad intelectual. Se resumen en la siguiente matriz de políticas:

| Categoría de Control | Política de Gobernanza Establecida | Impacto Operativo |
| :--- | :--- | :--- |
| **Imágenes Base Oficiales** | Solo se autoriza el uso de imágenes base limpias y optimizadas provistas en repositorios seguros de Harbor (ej. Debian o Alpine). | Estandariza el entorno (Golden Images). |
| **Seguridad (SAST)** | Ninguna imagen será distribuible si el escáner Trivy detecta vulnerabilidades Altas o Críticas sin mitigar. | Previene despliegues inseguros. |
| **Firma Criptográfica** | Los sistemas solo ejecutarán imágenes que posean una firma válida (Cosign/Sigstore) del Responsable de Imágenes. | Garantiza la autenticidad del código. |
| **Inmutabilidad** | Prohibido el uso de la etiqueta genérica `:latest`. Las imágenes deben tener versionado académico (ej. `ciclo-2026-B`) en repositorios inmutables. | Asegura que las prácticas no se rompan por actualizaciones sorpresa. |
| **Software Propietario** | Integración de un gestor de licencias concurrente (Key Server) en Kubernetes. | Limita las instancias activas según el contrato. |
| **Open Source (Copyleft)** | Licencias como GPL v3 o AGPL requieren auditoría previa y aprobación formal del Product Owner. | Evita el riesgo legal de contagio de código fuente propietario. |

### 9.5 Importancia de la trazabilidad
La trazabilidad permite auditar con precisión retrospectiva el origen, creador y estado de integridad de cualquier activo digital desplegado. En el ecosistema del laboratorio, esto significa conocer exactamente qué código fuente dio origen al contenedor, quién compiló la imagen, qué herramientas de terceros fueron añadidas y si se cuenta con los derechos de uso vigentes, facilitando análisis rápidos de causa raíz ante fallas de infraestructura o incidentes de seguridad.

<div align="center">
  <img src="./architecture/trazabilidad.jpg" alt="diagrama: Gobernanza de Seguridad y Firma Digital" width="80%">
</div>

Mediante el uso de etiquetas de metadatos integradas en los contenedores dentro de Harbor, es posible auditar de manera precisa los siguientes puntos:

* **Origen y autoría:** Quién construyó la imagen (identificando el GitLab runner ejecutor y el commit de origen en el repositorio).

* **Aprobación y confianza:** Quién validó y aprobó la publicación (verificable mediante la firma criptográfica del Responsable de Imágenes).

* **Estado de seguridad:** Qué vulnerabilidades específicas existían al momento exacto del despliegue en el catálogo.

* **Composición interna:** Qué dependencias, librerías y tipos de licencias de software componen la imagen.

* **Análisis de Causa Raíz:** Permite rastrear el origen del código causante de un incidente y parchar la imagen base de forma centralizada en minutos.

### 9.6 Beneficios para una empresa de software
El modelo diseñado para la universidad es escalable al sector corporativo, generando los siguientes beneficios:
*   **Reducción del Time-to-Market:** El aprovisionamiento de un entorno de desarrollo seguro pasa de tardar días a tomar solo unos minutos.
*   **Cumplimiento Normativo (Auditorías):** Facilita certificaciones internacionales de ciberseguridad (ISO/IEC 27001, SOC 2 y marcos COBIT).
*   **Eficiencia de Costos:** El uso de imágenes optimizadas y políticas automáticas de retención reducen los costos de almacenamiento en la nube.
*   **Mitigación de Riesgos:** Garantiza un entorno con cero multas por uso de software no licenciado y blinda frente a ataques a la cadena de suministro (Software Supply Chain Attacks).
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
