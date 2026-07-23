# Fases de Implementación

Cada fase se alinea con el calendario académico semestral de la universidad, para evitar que el trabajo quede interrumpido a mitad de ciclo por vacaciones o periodos de exámenes. El avance entre fases se basa en criterios de salida medibles, no únicamente en el tiempo transcurrido.

> **Qué se mejora respecto al documento original:** se agrega este párrafo introductorio. El documento original era solo una lista de fases sin ningún contexto.
> **Justificación:** no existía ningún criterio de alineación con el calendario académico, lo que podía interrumpir el trabajo a mitad de ciclo.

---

## Fase 0: Análisis y Diseño (1 mes)

> **Qué se mejora respecto al documento original:** se agregan entregables y criterios de aceptación. Antes la fase solo tenía nombre y duración.
> **Justificación:** sin entregables ni criterios de aceptación, la fase era un cronograma y no un plan de proyecto auditable.

**Entregables:**
- Diagrama de arquitectura (C4) validado.
- Backlog inicial priorizado (MoSCoW).
- Matriz de riesgos inicial.

**Criterios de Aceptación (Exit Gate):**
- [ ] Arquitectura aprobada por el Comité de Gobierno.
- [ ] Roles y Chapters conformados.
- [ ] Presupuesto de infraestructura base aprobado.

---

## Fase 1: Proyecto Universitario (4-6 meses / 2 semestres académicos)

> **Qué se mejora respecto al documento original:** se agrega la equivalencia en semestres académicos, entregables, criterios de aceptación y dependencia con la fase anterior.
> **Justificación:** no se aclaraba cómo el rango de 4-6 meses se alineaba con el calendario semestral, ni existía relación de dependencia explícita entre fases, generando ambigüedad y riesgo de cuello de botella.

**Entregables:**
- MVP de la plataforma en operación con al menos 1 curso piloto.
- Catálogo de imágenes funcional (creación, escaneo, firma, publicación).
- Documentación de procesos y matriz RACI validada.

**Criterios de Aceptación (Exit Gate):**
- [ ] Al menos 3 cursos usando la plataforma en producción sin incidentes críticos.
- [ ] KPIs definidos en `gestion-imagenes.md` cumplidos durante al menos un semestre completo.
- [ ] Plan de transferencia de conocimiento documentado (ver sección de Continuidad).

**Dependencia:** requiere el cierre formal de la Fase 0 (arquitectura aprobada).

---

## Fase 2: Proyecto Empresa (5-7 meses)

> **Qué se mejora respecto al documento original:** se agregan entregables, criterios de aceptación y dependencia con la Fase 1.
> **Justificación:** mismo hallazgo que en la Fase 1: faltaban entregables medibles y una relación de dependencia clara respecto a la fase anterior.

**Entregables:**
- Evolución de la plataforma a estándar empresarial (seguridad avanzada, HA completo).
- Squads de "Proyecto Empresa" conformados según el modelo organizacional ágil.

**Criterios de Aceptación (Exit Gate):**
- [ ] Arquitectura de alta disponibilidad validada mediante prueba de carga (efecto campana).
- [ ] DRP/BCP probado mediante simulacro de restauración.
- [ ] Auditoría de seguridad (DevSecOps) sin hallazgos críticos abiertos.

**Dependencia:** puede iniciar en paralelo a la etapa final de la Fase 1 si los squads de "Proyecto Empresa" ya están conformados, pero no puede cerrarse hasta que la Fase 1 haya validado el MVP en producción.

---

## Fase 3: Piloto en Laboratorios Reales

> **Qué se mejora respecto al documento original:** se agregan entregables, criterios de aceptación y un plan de rollback.
> **Justificación:** no existía un plan de rollback pese a que esta fase impacta directamente a estudiantes activos en clases reales, el momento de mayor riesgo de todo el proyecto.

**Entregables:**
- Piloto ejecutado en al menos un laboratorio físico completo, con estudiantes activos.
- Reporte de incidentes y lecciones aprendidas.

**Criterios de Aceptación (Exit Gate):**
- [ ] Cero interrupciones de clase no mitigadas por el plan de rollback.
- [ ] Satisfacción de usuarios ≥ 85% (según KPI definido).

**Plan de Rollback:**
Ante una falla crítica durante el piloto, se debe activar el entorno local de respaldo (ver `arquitectura.md`, sección DRP/BCP) para no interrumpir una clase en curso. El rollback debe estar documentado, ensayado previamente, y ser ejecutable por el Administrador de Laboratorio sin depender de un especialista externo.

---

## Fase 4: Mejora Continua y Documentación

> **Qué se mejora respecto al documento original:** se agregan entregables y criterio de evaluación.
> **Justificación:** la fase estaba nombrada pero sin ningún entregable ni forma de medir si realmente ocurre la mejora continua.

**Entregables:**
- Revisiones mensuales de procesos con el Chapter de Organización.
- Actualización semestral de la documentación (arquitectura, procesos, backlog).

**Criterios de Aceptación (Exit Gate):**
- Ciclo continuo, sin fecha de cierre; se evalúa mediante revisión trimestral del Comité de Gobierno.

---

## Gestión de Cambio Organizacional

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no se contemplaba ninguna actividad de capacitación o comunicación, pese a que la falta de gestión de cambio es la causa más común de fracaso en adopción de plataformas educativas.

*(Fase transversal, corre en paralelo a las Fases 1-3)*

- **Capacitación de Chapter Leads:** los profesores que lideren Chapters deben recibir una inducción a los procesos y herramientas de la plataforma antes de asumir el rol.
- **Comunicación a estudiantes:** guías rápidas y sesiones informativas al inicio de cada semestre.
- **Plan de transferencia de conocimiento entre cohortes:** documentación viva (wiki del proyecto) que permita a una nueva cohorte de estudiantes retomar el trabajo de la cohorte anterior sin pérdida de contexto, dado que la rotación estudiantil es de 1-2 semestres.

---

## Matriz de Riesgos

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no existía una matriz de riesgos propia del entorno universitario (rotación de estudiantes, disponibilidad docente, periodos de examen), pese a ser un factor determinante para la continuidad del proyecto.

| Riesgo | Probabilidad | Impacto | Mitigación |
|---|---|---|---|
| Rotación de estudiantes interrumpe continuidad del proyecto | Alta | Alto | Plan de transferencia de conocimiento, PO institucional permanente |
| Falla de infraestructura durante clase en curso | Media | Alto | Plan de rollback, entorno local de respaldo |
| Desalineación entre duración de fase y calendario académico | Alta | Medio | Fases ancladas a semestres, no a meses calendario |
| Falta de disponibilidad horaria de docentes (Chapter Leads) | Media | Medio | Formalización de horas dedicadas en carga docente |
| Vulnerabilidad crítica detectada a mitad de semestre | Media | Alto | Política de "fail the build" (ver `gestion-imagenes.md`) |

---

## Gobernanza del Proyecto

> **Sección nueva — no existía en el documento original.**
> **Justificación:** no había indicación de un Product Owner o comité de gobierno responsable de dar continuidad al proyecto entre cohortes de estudiantes que rotan cada 1-2 semestres.

- **Product Owner institucional:** un coordinador de carrera o Chapter Lead senior, con carácter permanente, que no rota con cada cohorte de estudiantes.
- **Comité de Gobierno:** integrado por el Product Owner institucional, Administrador de Laboratorio y representantes de Chapters, con checkpoints mensuales.
- **Presupuesto:** cada fase debe contar con una partida presupuestaria aprobada antes de su inicio (ver Anexo de Estimación de Costos).

---

<div style="color:red">

## Comentario del Integrante 1 — Revisión de `docs/fases-implementacion.md`

### ¿Qué está bien?

- La versión ampliada mejora considerablemente el listado original al incluir entregables, dependencias y criterios de salida por fase.
- Considera riesgos propios del entorno universitario, gestión del cambio, transferencia de conocimiento y continuidad entre cohortes.
- El piloto incluye un mecanismo de reversión y criterios relacionados con continuidad y satisfacción.
- Se reconoce que la mejora continua debe mantenerse después de la puesta en producción.

### ¿Qué está mal o puede mejorarse?

- Existe una inconsistencia al indicar que 4-6 meses equivalen a dos semestres académicos.
- En la Fase 1 se propone como entregable un curso piloto, pero como criterio de salida se exigen tres cursos; la transición no está explicada.
- No se indican fechas, responsables, esfuerzo, costos ni recursos asignados a cada actividad.
- La Fase 3 no tiene duración estimada y la Fase 4 no define una línea base para evaluar las mejoras.

### ¿Qué falta?

- Cronograma Gantt o roadmap con actividades, dependencias, responsables e hitos.
- Presupuesto por fase, plan de adquisiciones y disponibilidad del personal docente y técnico.
- Matriz RACI del proyecto y mecanismo formal para aprobar cambios de alcance.
- Plan detallado de pruebas funcionales, seguridad, rendimiento, aceptación del usuario y cierre.

### ¿Qué proponemos?

- Corregir las duraciones y expresar el calendario en semanas académicas, incluyendo exámenes y vacaciones.
- Asignar un responsable y un aprobador a cada entregable, con fecha comprometida y evidencia de aceptación.
- Elaborar un Gantt general y administrar la ejecución mediante un tablero Kanban con columnas Pendiente, En curso, En revisión y Terminado.
- Dividir el piloto en uno controlado con un curso y una ampliación posterior a tres cursos, condicionada al cumplimiento de los KPIs.
- Establecer revisiones quincenales, control de riesgos y un informe de cierre por cada fase.

</div>
