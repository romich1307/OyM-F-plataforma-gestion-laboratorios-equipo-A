# Procesos del Laboratorio - Plataforma Híbrida de Gestión

**Documento Técnico y Operativo**  
**Asignatura:** Organización y Métodos  
**Proyecto:** Plataforma Híbrida de Gestión de Laboratorios  
**Versión:** 1.0  
**Fecha:** Julio 2026

---

## 1. Introducción

Este documento define los **procesos principales** del laboratorio de computación, modelados bajo una perspectiva de **Organización y Métodos**. Se utilizan diagramas BPMN (Business Process Model and Notation) para representar claramente los flujos, roles, actividades y decisiones.

El objetivo es estandarizar el funcionamiento del laboratorio, reducir tiempos improductivos y garantizar trazabilidad.

---

## 2. Roles Principales (RACI)

| Rol                            | Responsabilidad Principal                     |
|-------------------------------|-----------------------------------------------|
| **Administrador de Laboratorio** | Gestión general y aprobación final           |
| **Responsable de Imágenes**    | Gestión del catálogo de contenedores         |
| **Docente / Product Owner**    | Solicitud y validación académica             |
| **Estudiante / Desarrollador** | Uso de recursos e imágenes                   |
| **Chapter de Organización**    | Definición y mejora continua de procesos     |

---

## 3. Procesos Principales (BPMN)

### 3.1 Proceso 1: Solicitud y Asignación de Recursos (Hardware)

```bpmn
Start → [Solicitud de Recursos] → ¿Recursos disponibles? 
   → Sí → [Asignación Temporal] → [Registro en Sistema] → End
   → No → [Notificación de Espera] → [Cola de Espera] → Revisar disponibilidad
```





# Auditoría de Analista BPMN (León Hatches)

## ¿Qué está bien?
Se tiene la siguiente lista de aspectos que se realizaron de manera correcta:
- Define un objetivo claro de estandarizar el funcionamiento, reducir tiempos improductivos y garantizar la trazabilidad.
- Menciona el uso de diagramas BPMN para representar flujos, roles, actividades y decisiones de forma clara.

## ¿Qué está mal o puede mejorarse?
Entre lo que puede mejorar, se tiene lo siguiente:
- La tabla de "Roles Principales (RACI)" es únicamente descriptiva y no realiza el cruce matricial real de responsabilidades.
- El documento está incompleto y se corta en el título "3.1 Proceso 1: Solicitud y Asignación de Recursos (Hardware)", suponiendo que es una versión obsoleta.

## ¿Qué falta?
Se obtiene la siguiente lista de carencias:
- Falta el desarrollo de los procesos y los diagramas prometidos en la introducción.

## ¿Qué proponemos?
Se propone los siguientes puntos:
- Construir tablas formales de actividades, entradas y salidas para cada proceso.
- Completar el documento integrando los diagramas BPMN 2.0 definitivos.