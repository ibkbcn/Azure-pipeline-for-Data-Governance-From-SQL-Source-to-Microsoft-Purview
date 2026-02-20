# Azure pipeline for Gobernance: From SQL Source to Microsoft Purview


## Objetivo del Proyecto
Implementar una solución de gobernanza de datos automatizada para el dataset de e-commerce (Olist), transformando datos técnicos en una base de datos Azure SQL en activos de negocio catalogados y clasificados dentro de Microsoft Purview.


## Arquitectura Técnica

Ingesta Inicial: Carga y sincronización de archivos CSV locales hacia Azure SQL Database.

Almacenamiento: Repositorio estructurado en Azure SQL como fuente única de verdad.

Motor de Gobernanza: Microsoft Purview, configurado para el descubrimiento de activos y linaje.

Seguridad y Permisos: Uso de Managed Identity (MSI) con permisos db_owner y VIEW DEFINITION para la extracción de metadatos.

Proceso: Ejecución de Scans automáticos con detección profunda para la clasificación de datos sensibles.


## Resultados
Catalogación: Catalogación automatizada de las tablas de Clientes, Pedidos, Productos y Pagos, eliminando el mantenimiento de diccionarios manuales y acelerando el descubrimiento de datos para los analistas.

Clasificación y Cumplimiento (GDPR): Identificación autónoma de datos sensibles de geolocalización y privacidad, permitiendo una gestión de riesgos proactiva y alineada con normativas internacionales.
