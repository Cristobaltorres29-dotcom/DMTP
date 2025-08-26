# Cómo usar las plantillas con tu correo

- Ya fijé el destinatario en el sitio: `to_email = cristobal29.ct@gmail.com`.
- En EmailJS:
  1. Crea un Template y pega `emailjs_template.html` (HTML) y `emailjs_template.txt` (Texto).
  2. En **To / Recipients** del template, usa la variable `{{to_email}}` (o asegúrate de que EmailJS la respete como destino).
  3. Variables requeridas: `to_email, nombre, telefono, correo, motivo, mensaje, cuerpo, timestamp`.
  4. Asunto sugerido: `Nueva consulta DMTP — {{motivo}} — {{nombre}}`.
  5. Reply-To: `{{correo}}` para responder al cliente.

- En `contacto.html` recuerda reemplazar:
  - `REEMPLAZAR_EMAILJS_PUBLIC_KEY`
  - `REEMPLAZAR_SERVICE_ID`
  - `REEMPLAZAR_TEMPLATE_ID`
  - (Opcional) `REEMPLAZAR_WEBHOOK_URL` para SMS/WhatsApp vía Zapier/IFTTT/Make.
