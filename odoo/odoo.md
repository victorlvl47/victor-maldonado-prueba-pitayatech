# Odoo

# 1. Gerencia de mercadeo
La gerencia de mercadeo necesita generar un reporte diario con las visitas de clientes a tiendas, este reporte debe contener:
- Cantidad de compras realizadas en el día.
- medio por el cual se enteraron de la empresa
- comentarios del cliente.

## Propuesta
Se utilizara principalmente la app de [CRM](https://www.odoo.com/app/crm) de Odoo, ya que permite gestionar las relaciones con los clientes y registrar todas las interacciones con ellos. Aquí se registrarán los detalles de las visitas de los clientes a las tiendas. Se va a configurar el módulo CRM para agregar campos adicionales para obtener la información requerida en el reporte, es decir agregar los campos para cantidad de compras realizadas en el día, Medio por el cual se enteraron de la empresa y Comentarios del cliente. Tambien se va a generar los reportes diarios con esta informacion, el reporte diario se va a diseñar para que muestre la cantidad de compras realizadas, el medio por el cual se enteraron de la empresa y los comentarios de los clientes para cada visita registrada. Vamos a automatizar el proceso de generacion de reportes para el final de cada dia.

## Tiempo estimado de desarrollo
El tiempo de desarrollo dependera del nivel de complejidad de la configuracion del app de CRM basado en los requerimiento de la gerencia de mercadeo y del diseño del informe. Asumiendo que este proyecto va quedar a cargo de un solo programador la estimacion seria de 4 semanas donde se incluye el análisis, diseño, desarrollo, pruebas y despliegue.



# 2. Encuesta de satisfacción
Como parte del servicio post-venta la gerencia de mercadeo, desea enviar a todossus
clientes una encuesta de satisfacción una vez que la **venta se encuentra facturada**.

## Propuesta
Se va a utilizar el app de [Sales](https://www.odoo.com/app/sales) de Odoo para gestionar el proceso de ventas y facturación, se registrarán todas las ventas realizadas y su estado, lo que nos permitirá identificar las ventas ya facturadas. Tambien se va a utilizar el app de [Surveys](https://www.odoo.com/app/surveys) de Odoo para para crear una encuesta personalizada que incluya las preguntas necesarias para evaluar la satisfacción del cliente. Este proceso va a ser automatico y se va a activar una vez que una venta se encuentre facturada, se enviará automáticamente la encuesta de satisfacción al cliente correspondiente a través del contacto preferido del cliente, correo electrónico, mensaje de texto, Direct Message, etc.

## Tiempo estimado de desarrollo
El tiempo de desarrollo para esta solución depende de la complejidad de la personalización de la encuesta y la configuración del flujo de trabajo automatizado. Una estimación inicial de 2 a 4 semanas, teniendo en cuenta el análisis, diseño, desarrollo, pruebas y despliegue.



# 3. Empresa Los 3 Amigos
Actualmente, para registrar los costos de gasolina, mantenimiento y depreciación 
devehículos en Odoo se genera un reporte de Excel desde esta aplicación y se registran 
manualmente uno por uno.
Se desea automatizar la carga de esta información a Odoo para evitar el trabajo manual.

## Propuesta
En el proceso actual en la empresa, el cueyo de botella es la carga manual de los 
reportes de excel al software Odoo. Para solucionar este problema y automatizar el 
proceso se propone los siguiente. Desarrollar un script en Python que se conecte a la 
aplicación externa, descargue los reportes de excel y los formatee adecuadamente para que puedan ser importados en Odoo. Odoo ofrece varias facilidades a los developers para realizar este tipo de integracion para [importa y exportar datos](https://www.odoo.com/documentation/16.0/applications/general/export_import_data.html). Se implementará una nueva funcionalidad para importar los datos desde el archivo generado por el nuevo script de integración que creamos. Se va aconfigurará una tarea programada ([Cron](https://odoo-development.readthedocs.io/en/latest/odoo/models/ir.cron.html)) y asi ejecutar automaticamente el nuevo script de integración y actualice automáticamente los registros de en Odoo.

## Tiempo estimado de desarrollo
El tiempo de desarrollo para esta solución esta en funcion de la complejidad de la integración con la aplicación externa y la configuración específica requerida. La estimación seria de 4 semanas, tomando en cuenta análisis, diseño, desarrollo, pruebas y despliegue.