# Sistema Automatizado de Reporting Operativo para E-commerce

He desarrollado un workflow en n8n para automatizar la generación de reportes diarios en operaciones de e-commerce. El sistema recopila datos desde Google Sheets sobre ventas, pedidos e incidencias, unifica la información, calcula métricas clave y genera un reporte profesional en formato HTML que se envía automáticamente por Gmail.

Además, guarda cada reporte en una pestaña histórica para mantener trazabilidad diaria de los resultados y facilitar el seguimiento operativo.

## Objetivo

Automatizar la generación de reportes operativos diarios para e-commerce a partir de múltiples fuentes de datos, reduciendo trabajo manual y mejorando la visibilidad sobre el rendimiento diario de la operación.

## Problema que resuelve

En operaciones de e-commerce, la información suele estar repartida entre varias hojas o fuentes separadas. Esto hace que preparar reportes diarios consuma tiempo, aumente el riesgo de errores y dificulte el seguimiento constante del negocio.

Este proyecto automatiza ese proceso para:

- leer ventas, pedidos e incidencias desde Google Sheets
- unificar datos operativos
- calcular métricas clave automáticamente
- generar un reporte HTML profesional
- enviar el reporte por Gmail
- guardar un histórico diario para trazabilidad

## Métricas generadas

El workflow calcula automáticamente:

- ventas totales
- número de ventas
- pedidos totales
- pedidos enviados
- incidencias totales
- incidencias abiertas
- estado general operativo

## Flujo del workflow

### 1) Ejecución programada
El workflow se ejecuta automáticamente cada día mediante un `Schedule Trigger`.

### 2) Lectura de datos
Se consultan tres pestañas de Google Sheets:

- Ventas
- Pedidos
- Incidencias

### 3) Unificación de información
Los datos se combinan usando nodos `Merge` para construir una vista operativa única.

### 4) Cálculo de métricas
Un nodo `Code` procesa la información y genera indicadores clave del día.

### 5) Generación del reporte
Otro nodo `Code` construye un email en HTML con formato profesional.

### 6) Envío automático por email
El reporte se envía automáticamente por Gmail al destinatario definido.

### 7) Guardado histórico
Las métricas diarias se almacenan en una pestaña de histórico para seguimiento y auditoría operativa.

## Buenas prácticas aplicadas

- Automatización programada
- Separación de fuentes de datos
- Procesamiento y agregación con JavaScript
- Generación dinámica de HTML
- Registro histórico para trazabilidad
- Diseño útil para reporting operativo real
- Estructura mantenible y escalable

## Herramientas utilizadas

- n8n
- Google Sheets
- Gmail
- JavaScript
- HTML
- Scheduled Workflows
- Data Processing

## Archivos del proyecto

- [workflow-export.json](./workflow-export.json)

## Captura principal

![Workflow Screenshot](./workflow-screenshot.png)

## Evidencias adicionales

![Email Report Preview](./email-report-preview.png)

![Report History Sheet](./report-history-sheet.png)

## Valor para portfolio

Este proyecto demuestra capacidad para construir automatizaciones orientadas a operaciones reales de e-commerce, especialmente en procesos donde reporting, visibilidad operativa y trazabilidad diaria son importantes.

Especialmente muestra experiencia en:

- automatización de reporting
- integración con Google Sheets
- procesamiento de datos
- generación de emails HTML
- scheduled workflows
- almacenamiento histórico de métricas

## Enfoque profesional

Este es el tipo de soluciones que quiero seguir creando: automatizaciones útiles, escalables y enfocadas en mejorar operaciones reales de e-commerce, reducir errores, mejorar el control de stock y acelerar la gestión de pedidos.
