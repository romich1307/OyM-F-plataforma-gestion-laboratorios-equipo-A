# Procesos y Organización del Laboratorio

**Documento Integral de Organización y Métodos**  
**Proyecto:** Plataforma Híbrida de Gestión de Laboratorios  
**Asignatura:** Organización y Métodos  
**Versión:** 1.0  
**Fecha:** Julio 2026

---

## 1. Introducción

Este documento presenta la **organización completa** y los **procesos clave** del laboratorio de computación. Su propósito es estandarizar el funcionamiento, reducir tiempos improductivos, garantizar trazabilidad y servir como referencia para la asignatura de **Organización y Métodos**.

Se incluyen descripciones detalladas, diagramas BPMN textuales, matriz RACI, indicadores y propuestas de mejora.

---

## 2. Estructura Organizacional Mínima

### Roles Principales

- **Administrador de Laboratorio**: Responsable general de la operación física y digital.
- **Responsable de Imágenes**: Gestor del catálogo de contenedores (Docker).
- **Chapter de Organización y Procesos**: Profesor líder (encargado de definir, documentar y mejorar procesos).
- **Docente / Product Owner**: Solicita y valida recursos por curso/proyecto.
- **Estudiante / Desarrollador**: Usuario final.
- **Chapter Leads Técnicos**: Profesores por especialidad (DevOps, Seguridad, etc.).

### Propuesta de Organización

Se recomienda un **Chapter de Organización y Procesos** (transversal) en lugar de un squad completo. Este Chapter trabajará junto con un **Rol de "Process Owner"** dentro de cada Squad técnico.

**Justificación**: Permite mantener los squads enfocados en desarrollo mientras se garantiza que los procesos sean prácticos y bien documentados.

---

## 3. Procesos Principales (con Descripción Detallada)

### 3.1 Proceso: Solicitud y Asignación de Recursos de Hardware

**Objetivo:** Gestionar de forma eficiente las computadoras, servidores e impresoras.

**Flujo BPMN (Textual):**

Start → Solicitud por Portal → Verificación Automática de Disponibilidad 
→ ¿Disponible? 
   → Sí → Aprobación Automática / Manual → Asignación + Notificación → Check-in (QR) → Uso → Check-out → Liberación → End
   → No → Notificación de Espera → Cola de Prioridad → Revisión Manual



**Descripción Detallada:**
1. El usuario inicia sesión y selecciona el recurso.
2. El sistema verifica disponibilidad en tiempo real.
3. Se registra el préstamo con fecha/hora de devolución.
4. Al llegar al laboratorio se realiza Check-in.

---

### 3.2 Proceso: Gestión del Catálogo de Imágenes de Contenedores (Core)

**Objetivo:** Proporcionar entornos estandarizados y trazables.

**Flujo BPMN (Textual):**

Start → Solicitud de Imagen (Estudiante/Docente)
→ Búsqueda Automática en Harbor
→ ¿Imagen Disponible y Actualizada?
   → Sí → Entrega de Enlace de Descarga → Uso Local / Laboratorio → End
   → No → Notificación al Responsable de Imágenes
      → Análisis (Oficial vs Crear)
      → Descarga / Creación de Imagen
      → Escaneo de Vulnerabilidades
      → Firma Digital
      → Aprobación
      → Publicación en Harbor
      → Notificación a Solicitante



**Descripción Detallada:**
- Toda imagen debe estar **escaneada y firmada**.
- Los estudiantes pueden descargar la imagen oficial y ejecutarla en su computadora personal con Docker o Podman.
- Se mantiene un historial completo de versiones.

---

### 3.3 Proceso: Actualización y Mantenimiento de Imágenes

**Flujo BPMN:**

Start → Detección Automática de Nueva Versión
→ Pipeline de Rebuild
→ Escaneo de Seguridad
→ ¿Requiere Aprobación Manual?
   → Sí → Revisión por Responsable → Aprobación/Rechazo
   → No → Actualización Automática
→ Publicación → Notificación a Usuarios Activos → End



---

### 3.4 Proceso: Reserva y Uso de Laboratorio

**Flujo BPMN:**

Start → Login → Seleccionar Horario y Equipo
→ Validación de Disponibilidad
→ Reserva Confirmada → Recordatorio 15 min antes
→ Check-in en Laboratorio → Uso → Check-out → Liberación Automática



---

## 4. Matriz RACI General

| Actividad / Proceso                    | Administrador Lab | Responsable Imágenes | Docente | Estudiante | Chapter Organización |
|---------------------------------------|-------------------|----------------------|---------|----------|----------------------|
| Solicitud de Recursos Hardware        | A                 | I                    | C       | R        | C                    |
| Solicitud y Aprobación de Imágenes    | A                 | R                    | C       | R        | C                    |
| Creación de Nueva Imagen              | C                 | R/A                  | C       | I        | C                    |
| Reserva de Equipos                    | A                 | I                    | C       | R        | I                    |
| Actualización de Imágenes             | I                 | R                    | C       | I        | C                    |
| Definición y Mejora de Procesos       | C                 | C                    | C       | I        | R/A                  |

---

## 5. Indicadores de Desempeño (KPIs)

- Tiempo promedio de aprobación de nueva imagen: **≤ 48 horas**
- Porcentaje de solicitudes resueltas automáticamente: **≥ 70%**
- Tiempo promedio de configuración de entorno por estudiante: **≤ 15 minutos**
- Tasa de utilización de imágenes oficiales: **≥ 75%**
- Nivel de satisfacción de usuarios (Encuesta): **≥ 85%**
- Tiempo promedio de reserva de equipo: **≤ 5 minutos**

---

## 6. Mejora Continua y Recomendaciones

- Realizar **revisiones mensuales** de procesos con el Chapter de Organización.
- Utilizar herramientas como **Draw.io, Bizagi o Camunda** para mantener diagramas BPMN actualizados.
- Implementar **automatización progresiva** de decisiones mediante reglas de negocio.
- Crear un **manual de usuario** y **guías rápidas** para estudiantes.
- Establecer un **comité de procesos** (Administrador + Chapter Leads + Estudiantes representantes).

**Próximos Pasos:**
1. Modelar todos los diagramas BPMN en herramienta gráfica.
2. Validación del documento con docentes y administradores.
3. Integración de flujos automatizados en la plataforma.

---

**Este documento integra toda la parte de Organización y Procesos del Laboratorio.**  
Está diseñado para ser entregado como **trabajo de curso de Organización y Métodos**.

---

¿Deseas que agregue más procesos (ej. Gestión de Incidentes, Onboarding de Nuevos Usuarios, Cierre de Semestre, etc.) o que prepare una versión con PlantUML para generar diagramas reales?






# Auditoría de Analista BPMN (León Hatches)

## ¿Qué está bien?
Se tiene la siguiente lista de aspectos que se realizaron de manera correcta:
- Identifica correctamente a los actores clave (Administrador de lab, Responsable de Imágenes, Docente, Estudiante) y cuenta con una matriz RACI.
- Integra correctamente el concepto de "Chapter de Organización" para mantener la mejora continua sin entorpecer a los equipos técnicos.
- Además, propone un set inicial de KPIs, lo cual es excelente para la medición del desempeño.

## ¿Qué está mal o puede mejorarse?
Entre lo que puede mejorar, se tiene lo siguiente:
- La representación de los procesos BPMN es exclusivamente textual, por lo que no cumple con el estándar visual formal para el modelado de procesos.
- La matriz RACI asigna el rol de "R/A" (Responsable y Aprobador) al Responsable de Imágenes en la creación de nuevas imágenes, rompiendo el principio de segregación de funciones.

## ¿Qué falta?
Se obtiene la siguiente lista de carencias:
- Faltan los diagramas BPMN reales en herramientas gráficas.
- Falta incluir flujos de procesos de soporte críticos sugeridos en el mismo documento, como Gestión de Incidentes y Onboarding de Nuevos Usuarios.

## ¿Qué proponemos?
Se propone los siguientes puntos:
- Rediseñar la Matriz RACI separando claramente quién ejecuta (R) y quién aprueba (A).
- Elaborar fichas técnicas detalladas para los KPIs propuestos.
- Modelar gráficamente todos los procesos.

---

# Auditoría de Analista Organizacional (Jose Morocco)

<div style="color:red;">

*Nota: Esta sección analiza exclusivamente la Matriz RACI de la Sección 4, cuya evaluación recae en el rol de Analista Organizacional.*

</div>

## ¿Qué está bien?
<div style="color:red;">

Se tiene la siguiente lista de aspectos que se realizaron de manera correcta:

- El uso de la metodología RACI refleja correctamente la autoridad formal del Administrador.
- Asignar R/A al Responsable de Imágenes en su creación es correcto por su propiedad técnica.

</div>

## ¿Qué está mal o puede mejorarse?
<div style="color:red;">

Entre lo que puede mejorar, se tiene lo siguiente:

- Agrupar "Solicitud" y "Aprobación" en una sola fila destruye la claridad: solicitar no es aprobar.
- El Chapter de Organización figura como Consulted (C) sin ningún mecanismo definido de consulta.
- El Docente está subutilizado (solo Consulted) cuando él origina las solicitudes de nuevas imágenes.

</div>

## ¿Qué falta?
<div style="color:red;">

Se obtiene la siguiente lista de carencias:

- Faltan columnas para "Chapter Leads Técnicos" y "Encargado de Laboratorio", activos pero ausentes.
- Faltan procesos críticos no mapeados: Gestión de Incidentes, Auditoría y Onboarding/Offboarding.
- Faltan las matrices complementarias de Comunicación y de Escalamiento (niveles N0 a N4).

</div>

## ¿Qué proponemos?
<div style="color:red;">

Se propone los siguientes puntos:

- Desdoblar "Solicitud y Aprobación de Imágenes" en dos filas independientes con actores correctos.
- Presentar una Matriz RACI corregida con 15 actividades y 7 roles, incluyendo lo faltante.
- Crear documentos formales de Matriz de Comunicación y Matriz de Escalamiento como entregables.

</div>