Order & Inventory Management Automation
Este proyecto es un workflow desarrollado en n8n para automatizar la gestión de pedidos e inventario en un escenario de e-commerce.
El flujo recibe pedidos a través de un webhook, valida los datos obligatorios, consulta el stock disponible en Google Sheets, actualiza automáticamente el inventario cuando hay unidades suficientes y envía una alerta por Gmail cuando no hay stock disponible. También gestiona pedidos inválidos y devuelve respuestas JSON estructuradas para cada caso.
Funcionalidades principales
Recibe pedidos mediante un webhook POST.
Valida los campos obligatorios del pedido.
Consulta el stock del producto en Google Sheets.
Comprueba la disponibilidad usando lógica en JavaScript.
Actualiza el inventario automáticamente cuando hay stock suficiente.
Envía alertas por Gmail cuando el stock es insuficiente.
Devuelve respuestas estructuradas para:
pedidos procesados correctamente,
pedidos sin stock,
pedidos inválidos.
Herramientas utilizadas
n8n.
Webhooks.
Google Sheets.
Gmail.
JavaScript.
Postman.
Lógica del workflow
Recibir nuevo pedido.
Validar los datos del pedido.
Buscar el stock del producto.
Comprobar si hay stock suficiente.
Si hay stock, actualizar inventario.
Si no hay stock, enviar alerta por email.
Devolver una respuesta estructurada según el resultado.
Valor del proyecto
Este proyecto demuestra automatización de procesos, validación de datos, integración con APIs, lógica condicional, gestión de inventario y manejo de errores en un contexto de e-commerce.
