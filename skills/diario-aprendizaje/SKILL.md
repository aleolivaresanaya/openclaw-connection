---
name: diario-aprendizaje
description: Organiza los apuntes reales de estudio de Ale y guarda una entrada en Google Docs. Usar cuando Ale pida registrar lo aprendido, guardar sus apuntes o crear una entrada de su diario de aprendizaje.
---

# Diario de aprendizaje de Ale

## Contexto y requisitos
- Aplicar IDENTITY.md, SOUL.md, AGENTS.md, USER.md y TOOLS.md.
- Mantener la voz de Nova: español directo, explicaciones sencillas y pasos concretos.
- Usar únicamente la conexión existente de Zapier MCP mediante mcporter.
- No instalar herramientas ni configurar conexiones nuevas.

## Procedimiento
1. Recibir los apuntes de Ale: tema estudiado, aprendizajes y dudas.
2. Si faltan apuntes, solicitarlos. No inventar lo que Ale aprendió.
3. Confirmar la fecha de la entrada si no quedó indicada inequívocamente.
4. Preparar estas secciones:
   - Tema.
   - Lo que aprendí.
   - Ejemplo relacionado con mis apuntes.
   - Dudas pendientes.
   - Próximo paso pequeño y realizable.
5. Distinguir cualquier ejemplo explicativo añadido de lo que Ale afirmó haber aprendido.
6. Consultar el esquema actual de google_docs_create_document_from_text y la forma de invocarlo mediante mcporter.
7. Usar title: "Diario de aprendizaje de Ale - YYYY-MM-DD" y file: contenido de la entrada. Verificar los campos contra el esquema disponible; no adivinar argumentos.
8. Usar My Google Drive y su carpeta raíz únicamente si esos valores predeterminados siguen configurados. No cambiar permisos ni compartir el documento.
9. Crear un documento por entrada cuando Ale haya solicitado guardarla. Si solo pidió un borrador, mostrarlo sin crear nada.
10. Comprobar la respuesta del servicio y devolver el enlace o identificador real, con una confirmación breve de Nova.

## Resultado verificable
- El servicio confirma la creación del documento con el título y contenido solicitados.
- Ale puede abrirlo y comprobar que refleja sus apuntes.
- Una respuesta de creación confirma la operación, pero no demuestra por sí sola que se hayan comprobado sus permisos.

## Casos especiales
- Si falla la conexión, presentar el borrador e informar que no se guardó.
- Si una solicitud agota el tiempo de espera y no se sabe si creó el documento, verificar antes de reintentar; si no se puede, preguntar a Ale para evitar duplicados.
- No repetir una creación que ya tenga confirmación de éxito.
- No incluir credenciales ni datos sensibles de terceros.
