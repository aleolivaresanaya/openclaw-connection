---
name: plan-estudio
description: Organiza los pendientes reales de estudio de Ale según prioridades y disponibilidad. Usar cuando pida planificar sus estudios o reservar bloques de estudio en Google Calendar.
---

# Plan de estudio de Ale

## Contexto y requisitos
- Aplicar IDENTITY.md, SOUL.md, AGENTS.md, USER.md y TOOLS.md.
- Responder como Nova: español claro, directo y práctico.
- Utilizar únicamente Google Calendar mediante la conexión existente de Zapier MCP y mcporter.
- Usar America/Mexico_City para interpretar fechas y horarios.

## Procedimiento
1. Recibir pendientes, prioridades, fechas límite y tiempo disponible de Ale.
2. Pedir los datos imprescindibles que falten. Convertir fechas relativas en fechas concretas y confirmarlas si son ambiguas.
3. Preparar un plan con tarea, objetivo concreto, prioridad, fecha, hora y duración.
4. No superar la disponibilidad indicada. No superponer los bloques propuestos entre sí.
5. Consultar el calendario personal predeterminado mediante las herramientas existentes. No usar calendarios de festivos ni inventar calendarid.
6. Si existe una acción para consultar eventos, comprobar conflictos. Si no existe, advertir que no se verificaron y pedir a Ale que confirme disponibilidad.
7. Mostrar los bloques y el calendario de destino. Pedir aprobación explícita antes de crear eventos.
8. Si Ale solo solicita un plan, entregar la propuesta sin crear eventos.
9. Tras la aprobación, consultar el esquema actual de google_calendar_create_detailed_event y su forma de invocación mediante mcporter.
10. Crear únicamente los bloques aprobados usando:
    - calendarid: identificador verificado del calendario personal.
    - start__dateTime: inicio con fecha y zona horaria inequívocas.
    - end__dateTime: fin posterior al inicio.
    - summary: "Estudio - " seguido de la tarea.
    - description: objetivo concreto y contexto necesario.
11. No añadir invitados, videollamadas ni recurrencias salvo solicitud explícita.
12. Comprobar cada respuesta y devolver un resumen con los eventos creados y sus enlaces o identificadores reales.

## Resultado verificable
- Los eventos aparecen en el calendario personal con las fechas, horas y duración aprobadas.
- Ale puede comprobarlos en Calendar.
- El resumen distingue propuesta, eventos creados y operaciones fallidas.

## Casos especiales
- Si no se puede identificar el calendario, preguntar antes de crear.
- Si hay conflictos, proponer alternativas y pedir aprobación.
- Si falta tiempo, priorizar y señalar lo que queda pendiente.
- Si falla una creación, conservar los eventos ya confirmados e informar del resultado parcial.
- Ante un timeout incierto, comprobar si el evento existe antes de reintentar; si no se puede comprobar, consultar a Ale.
- No repetir eventos cuya creación ya se confirmó.
- No configurar nuevas APIs, conexiones OAuth ni programaciones automáticas.
- No publicar correos personales, identificadores privados ni credenciales en evidencias públicas.
