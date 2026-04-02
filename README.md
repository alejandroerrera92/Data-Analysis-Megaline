# Data-Analysis-Megaline
Análisis de datos para Megaline: Compara el comportamiento de consumo y los ingresos generados por los planes 'Surf' y 'Ultimate' para optimizar las estrategias de marketing.
 Análisis Estadístico para Detectar Patrones y Outliers en Megaline

## Descripción del Proyecto

Este proyecto se centra en el análisis de datos de clientes para el operador de telecomunicaciones Megaline. El objetivo principal es determinar cuál de sus dos tarifas de prepago, 'Surf' o 'Ultimate', genera mayores ingresos para la empresa. A través de un análisis exploratorio de datos (EDA) y técnicas estadísticas, se investigará el comportamiento de consumo de los clientes en relación con llamadas, mensajes SMS y uso de internet. Los resultados de este análisis ayudarán al departamento comercial a ajustar su presupuesto de publicidad y estrategias de marketing.

## Objetivos Académicos

*   Demostrar un ejemplo de resumen estadístico aplicado al dataset de Megaline.
*   Cargar el reporte de análisis a GitHub.

## Descripción de los Datos

Se dispone de datos de 500 clientes de Megaline, incluyendo:

*   **`megaline_calls.csv`**: Información sobre las llamadas (duración, fecha).
*   **`megaline_internet.csv`**: Datos de uso de internet (MB usados, fecha).
*   **`megaline_messages.csv`**: Detalles de los mensajes de texto enviados (fecha).
*   **`megaline_plans.csv`**: Descripción de las tarifas 'Surf' y 'Ultimate' (costo mensual, límites de minutos, mensajes, GB).
*   **`megaline_users.csv`**: Información de los clientes (edad, ciudad, plan, fecha de registro).

Megaline redondea los segundos a minutos (hacia arriba) para las llamadas y los megabytes a gigabytes (hacia arriba) para el tráfico web mensual.

## Metodología

1.  **Carga de Datos**: Importación de los datasets proporcionados.
2.  **Análisis Preliminar y Limpieza de Datos**:
    *   Inspección de la estructura de cada dataset (`.info()`, `.head()`).
    *   Tratamiento de valores nulos y duplicados.
    *   Conversión de tipos de datos (`datetime`) y extracción de información relevante (ej. año-mes).
    *   Redondeo de la duración de las llamadas a minutos enteros (hacia arriba).
    *   Calculo de uso de internet en GB (redondeando hacia arriba el total mensual).
3.  **Agrupación y Análisis Estadístico por Consumo (Mes-Usuario)**:
    *   Cálculo del consumo mensual de llamadas, mensajes e internet por cada usuario.
    *   Análisis de la distribución de cada tipo de consumo (histogramas, boxplots).
    *   Identificación y discusión de outliers mediante el método IQR.
4.  **Segmentación de Usuarios**:
    *   Cálculo del consumo promedio de GB, mensajes y minutos por mes/usuario, agrupado por `plan`.
    *   Cálculo del consumo promedio de GB, mensajes y minutos por mes/usuario, agrupado por `ciudad`.
    *   Discusión de las diferencias de consumo entre planes y ciudades.
5.  **Facturación (Opcional)**:
    *   Estimación de la facturación mensual por usuario considerando su plan y consumo.
    *   Análisis de diferencias en la facturación entre planes.

## Resultados Clave (Ejemplos)

*   Se observa que el plan 'Ultimate' tiende a tener un consumo promedio de GB ligeramente superior al plan 'Surf'. (Este es un ejemplo, los resultados reales se derivarán del análisis).
*   La distribución del envío de mensajes muestra una concentración en valores bajos con algunos outliers de alto volumen.

## Conclusiones

[Se completarán las conclusiones finales una vez finalizado el análisis, destacando qué plan genera más ingresos y por qué, así como cualquier patrón de consumo interesante o recomendaciones para Megaline.]
