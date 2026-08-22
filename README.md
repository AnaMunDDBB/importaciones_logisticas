# Sistema de Gestión de Importaciones y Logística
**Base de datos relacional para la optimización de la cadena de suministro en comercio internacional.**

Este repositorio contiene el modelo de datos, la población y las consultas de análisis para una empresa importadora de electrónicos. El objetivo es centralizar información de proveedores y tarifas de flete para tomar decisiones de compra basadas en **costo, tiempo de tránsito y riesgo geopolítico en el uso de transporte marítimo**.

## Modelo de Datos
- **Proveedores:** 200 registros con datos de países asiáticos (China, Vietnam, India, Corea del Sur, Taiwán). 
- **Tarifas de Flete:** 500 rutas marítimas con costos, tiempos de tránsito y niveles de riesgo incrementales (1 = bajo, 2 = medio, 3 = alto).

## Tecnologías Utilizadas
- **Motor:** MySQL / MariaDB.
- **Entorno:** VS Code con extensión MySQL.
- **Técnicas:** Diseño de esquemas relacionales, `WITH RECURSIVE` para generación de datos masivos y buenas prácticas de normalización.

## Próximos Pasos (Roadmap del Proyecto)
- Análisis de costo total por unidad.
- Dashboards en Power BI para seguimiento de KPIs logísticos (OTIF, Lead Time).
- Simulación de escenarios de riesgo (bloqueos de rutas, aumentos de flete).

## Estructura del Repositorio
- `schemas.sql`: Creación de tablas y relaciones.
- `populate.sql`: Inserción masiva de datos con `WITH RECURSIVE`.
- `queries.sql`: Consultas de negocio (en desarrollo).
- 
[Schemas.sql](https://github.com/user-attachments/files/31336127/Schemas.sql)
[populate.sql](https://github.com/user-attachments/files/31336126/populate.sql)
