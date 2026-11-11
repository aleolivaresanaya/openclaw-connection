# Diseño de skills personales de Nova

## 1. diario-aprendizaje

### ¿Qué hace?
Convierte mis apuntes de estudio en una entrada estructurada y la guarda en Google Docs mediante la conexión existente de Zapier.

### ¿Qué input necesita?
Le proporciono qué estudié, qué entendí y qué dudas tengo, en texto libre o una lista. Si no indico fecha, debe confirmar qué fecha corresponde antes de guardar. USER.md aporta mi contexto de 4Geeks y mi preferencia por explicaciones sencillas; SOUL.md define el tono y TOOLS.md los destinos y herramientas.

### ¿Cómo es un buen output?
Un documento privado titulado "Diario de aprendizaje de Ale - YYYY-MM-DD", con tema, aprendizajes, ejemplo basado en mis notas, dudas y siguiente paso. No inventa aprendizajes. Si solo está disponible crear documentos, genera uno por entrada. Devuelve el enlace o identificador recibido del servicio; yo abro el documento y compruebo su contenido. Si falla la conexión, conserva el borrador y no afirma que se guardó.

## 2. plan-estudio

### ¿Qué hace?
Organiza mis pendientes de estudio en un plan realista y crea bloques en Google Calendar después de que apruebe los horarios.

### ¿Qué input necesita?
Le proporciono pendientes, prioridades, fechas límite y franjas disponibles con fechas concretas. USER.md aporta mi contexto y zona horaria America/Mexico_City. No presupone acceso al portal de 4Geeks. Si no puede consultar Calendar con las herramientas existentes, me pide confirmar disponibilidad y advierte que no verificó conflictos.

### ¿Cómo es un buen output?
Un plan breve con prioridad, tarea, fecha, hora y duración, sin superar el tiempo disponible. Primero muestra la propuesta y solicita aprobación para los eventos concretos. Después crea los bloques aprobados usando la conexión existente, sin invitados. Devuelve los identificadores o enlaces disponibles y distingue eventos creados de fallidos. Yo verifico fechas, horas y duración en Calendar. No repite una creación si ya tiene confirmación de éxito.

## Reglas compartidas
- Usar únicamente las conexiones actuales; no crear APIs ni OAuth nuevos.
- Aplicar IDENTITY.md, SOUL.md, AGENTS.md, USER.md y TOOLS.md.
- No incluir credenciales ni datos sensibles en evidencias públicas.
- Probar cada skill con información real proporcionada por Ale.
- Registrar resultados verificables, sin confundir un borrador con una acción completada.
- Las skills se activan a petición; no incluyen programación automática.
