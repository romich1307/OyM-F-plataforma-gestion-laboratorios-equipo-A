Start → [Inicio de Sesión] → [Seleccionar Equipo] 
   → ¿Disponible?
      → Sí → [Reservar por Horario] → [Check-in con Código QR] → [Uso] → [Check-out] → End
      → No → [Ver Alternativas o Esperar]





# Auditoría de Analista BPMN (León Hatches)

## ¿Qué está bien?
Se tiene la siguiente lista de aspectos que se realizaron de manera correcta:
- Cubre todo el ciclo de uso e implementa un mecanismo de control físico mediante un Check-in con Código QR.

## ¿Qué está mal o puede mejorarse?
Entre lo que puede mejorar, se tiene lo siguiente:
- La representación es solo texto en lugar de un diagrama formal.
- La ruta alternativa cuando no hay equipos disponibles finaliza en un callejón sin salida ("Ver Alternativas o Esperar") sin ofrecer una resolución sistémica clara.

## ¿Qué falta?
Se obtiene la siguiente lista de carencias:
- Falta un manejo de excepciones de tiempo, como definir qué ocurre si el usuario reserva pero no realiza el Check-in.

## ¿Qué proponemos?
Se propone los siguientes puntos:
- Modelar el proceso de forma gráfica bajo el estándar BPMN.
- Añadir un evento intermedio de tiempo ("Timer Event") en el BPMN que libere el equipo automáticamente si no se registra el Check-in en un tiempo prudencial.