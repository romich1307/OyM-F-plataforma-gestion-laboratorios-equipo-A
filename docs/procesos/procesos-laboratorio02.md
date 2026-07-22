Start → [Solicitud de Imagen] → [Búsqueda Automática en Harbor]
   → ¿Existe y está actualizada?
      → Sí → [Entrega de Imagen] → [Descarga Local] → End
      → No → [Notificación al Responsable de Imágenes]
         → [Búsqueda Imagen Oficial] → ¿Existe oficial?
            → Sí → [Importar + Escanear] → [Aprobación] → [Publicar]
            → No → [Crear Imagen Personalizada] → [Escaneo Seguridad] → [Aprobación] → [Publicar]





# Auditoría de Analista BPMN (León Hatches)

## ¿Qué está bien?
Se tiene la siguiente lista de aspectos que se realizaron de manera correcta:
- Contempla pasos de seguridad fundamentales, incluyendo un escaneo de vulnerabilidades y una aprobación antes de publicar la imagen.
- Separa la lógica entre encontrar una imagen oficial existente y tener que crear una imagen personalizada.

## ¿Qué está mal o puede mejorarse?
Entre lo que puede mejorar, se tiene lo siguiente:
- La representación es solo texto en lugar de un diagrama formal.

## ¿Qué falta?
Se obtiene la siguiente lista de carencias:
- Falta un camino de rechazo para el "Escaneo Seguridad", asumiendo que siempre será exitoso y pasará a la aprobación.
- Falta la definición de "Pools" y "Lanes" para los actores involucrados.

## ¿Qué proponemos?
Se propone los siguientes puntos:
- Modelar el proceso de forma gráfica bajo el estándar BPMN.
- Diseñar el flujo visual utilizando carriles separados para el Docente/Estudiante, el Sistema y el Responsable de Imágenes.
- Agregar compuertas lógicas (XOR) para manejar los fallos en el escaneo de seguridad.