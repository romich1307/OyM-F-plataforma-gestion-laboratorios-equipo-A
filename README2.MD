# Plataforma Híbrida de Gestión de Laboratorios de Computación

**Proyecto Académico-Empresarial**  
**Carrera de Sistemas / Ingeniería de Software**  
**Universidad [Nombre]**  
**Versión:** 1.0  
**Fecha:** Julio 2026

## Tabla de Contenidos

- [Introducción](README.md#introducción)
- [Problemática Común](#problemática-común)
- [Objetivos](#objetivos)
- [Justificación y Beneficios](#justificación-y-beneficios)
- [Modelo Organizacional](#modelo-organizacional-ágil-spotify-adaptado)
- [Arquitectura](#arquitectura-técnica-propuesta)
- [Fases del Proyecto](#fases-de-implementación)

---

## Introducción

Este proyecto busca desarrollar una **plataforma híbrida** (local + nube) para la gestión integral de laboratorios de computación, aplicable en universidades y empresas de software.

---

## Problemática Común

- Pérdida de tiempo en instalaciones manuales por parte de estudiantes y administradores.
- Entornos no estandarizados entre computadoras.
- Falta de trazabilidad del software utilizado.
- Dificultad para replicar el entorno del laboratorio en las computadoras personales de los alumnos.
- Gestión ineficiente de hardware y recursos.

---

## Objetivos

**General:** Desarrollar una plataforma que estandarice, automatice y trace los entornos de desarrollo en laboratorios.

**Específicos:**
- Gestión centralizada de hardware y usuarios.
- Catálogo de imágenes de contenedores (Docker) con procesos automáticos.
- Trazabilidad completa del software.
- Posibilidad de que los alumnos descarguen y usen las mismas imágenes en sus PCs.
- Dos versiones: Académica y Empresarial (con estándares más altos).

---

## Justificación y Beneficios

- **Universidad:** Ahorro de tiempo para estudiantes y administradores. Entornos reproducibles.
- **Industria:** Formación con estándares profesionales reales.
- **Trazabilidad:** Registro auditable de todas las imágenes y herramientas utilizadas.

---

## Modelo Organizacional Ágil (Spotify Adaptado)

Ver detalle completo en: [`docs/organizacion-agil.md`](docs/organizacion-agil.md)

## Arquitectura Técnica Propuesta

Ver detalle completo en: [`docs/arquitectura.md`](docs/arquitectura.md)

## Gestión de Imágenes y Trazabilidad

Ver detalle completo en: [`docs/gestion-imagenes.md`](docs/gestion-imagenes.md)

## Fases de Implementación

Ver detalle completo en: [`docs/fases-implementacion.md`](docs/fases-implementacion.md)

## Anexos

- [Requisitos de Roles y Habilidades](docs/roles-habilidades.md)
- [Cuadro Comparativo de Conocimientos](docs/roles-habilidades.md#cuadro-comparativo)
- [Plan de Dedicación](docs/plan-dedicacion.md)

---

**Estado:** Propuesta Inicial  
**Licencia:** MIT

---

<div style="color:red">

## Comentario del Integrante 1 — Revisión de `README2.MD`

### ¿Qué está bien?

- Funciona como una síntesis rápida de la propuesta y permite identificar el problema, los objetivos y los beneficios principales.
- Su estructura breve facilita que una persona interesada conozca el proyecto antes de revisar la documentación detallada.
- Incluye enlaces hacia documentos especializados de organización, arquitectura, gestión de imágenes y fases.

### ¿Qué está mal o puede mejorarse?

- Repite gran parte del `README.md`, lo que puede provocar versiones contradictorias cuando uno se actualice y el otro no.
- La tabla de contenidos combina enlaces internos y externos de forma inconsistente.
- El resumen no explica el alcance mínimo viable, los usuarios principales ni el estado real de avance.
- El enlace a `docs/gestion-imagenes.md` está roto porque ese archivo ya no existe con ese nombre en la versión actual del repositorio.

### ¿Qué falta?

- Una indicación clara de que este archivo es un resumen ejecutivo y de cuál documento constituye la fuente oficial.
- Responsables del proyecto, fecha de última actualización y próximos hitos.
- Indicadores resumidos de éxito, riesgos principales y diferenciación entre la versión académica y empresarial.
- Corrección o eliminación de enlaces hacia `docs/roles-habilidades.md`, que actualmente no existe.

### ¿Qué proponemos?

- Usar `README.md` como única portada oficial y convertir `README2.MD` en un resumen ejecutivo enlazado, o eliminarlo para evitar duplicidad.
- Añadir una tabla breve con alcance, beneficiarios, entregables, responsable y estado.
- Validar automáticamente los enlaces internos del repositorio antes de cada entrega.
- Corregir la codificación de caracteres y actualizar los enlaces conforme cambien los nombres de los archivos.

</div>
