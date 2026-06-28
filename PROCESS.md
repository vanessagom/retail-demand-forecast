# PROCESS

## Objetivo

Documentar el proceso seguido durante el desarrollo del proyecto, incluyendo la metodología aplicada, las herramientas utilizadas y las principales decisiones técnicas tomadas durante la construcción del modelo de forecasting.

## Enfoque del proyecto

El proyecto aborda un problema de **forecasting de demanda diaria** a nivel **tienda–categoría**. Este nivel de granularidad permite generar predicciones accionables para apoyar decisiones relacionadas con inventario, asignación de personal, abastecimiento y planeación promocional.

El desarrollo siguió un enfoque iterativo, donde las decisiones de modelado fueron sustentadas en evidencia obtenida durante el análisis exploratorio y en la evaluación continua del desempeño de los modelos.

## Metodología

El flujo de trabajo seguido fue el siguiente:

1. Comprensión del problema de negocio.
2. Carga y validación inicial de datos.
3. Análisis exploratorio de datos (EDA).
4. Evaluación de calidad de datos.
5. Ingeniería de variables.
6. Construcción y comparación de modelos de forecasting.
7. Interpretación del modelo mediante importancia de variables.
8. Evaluación sobre datos no observados.
9. Construcción de un caso de uso orientado al negocio.

## Estructura del proyecto

El proyecto se desarrolló utilizando notebooks de Jupyter con propósitos diferenciados:

- **`explore_analysis.ipynb`**: análisis exploratorio, generación de hipótesis e identificación de los principales factores asociados a la demanda.
- **`train_forecast_model.ipynb`**: construcción del dataset de modelado, ingeniería de variables, entrenamiento, evaluación e interpretación de los modelos de forecasting.

## Registro de decisiones

| Decisión | Justificación |
|---|---|
| Modelar la demanda a nivel tienda–categoría | Permite generar predicciones más específicas y útiles para la operación. |
| Utilizar `total_transactions` como variable objetivo | Representa una aproximación directa a la demanda diaria de cada tienda y categoría. |
| Excluir variables como `sales_amount`, `units_sold`, `average_ticket` y `replenishment_signal` | No estarían disponibles al momento de realizar una predicción futura o podrían introducir *data leakage*. |
| Construir un modelo baseline antes de modelos más complejos | Permite establecer una referencia objetiva para evaluar si los modelos de Machine Learning aportan una mejora real. |
| Comparar Regresión Lineal y LightGBM | Evaluar tanto un modelo interpretable como uno capaz de capturar relaciones no lineales. |
| Probar distintos esquemas de división temporal | Analizar la sensibilidad del modelo al diseño experimental y comprender el impacto del esquema de validación en las métricas obtenidas. |
| Mantener un enfoque orientado al negocio | Todas las decisiones de modelado se justifican con base en los hallazgos del análisis exploratorio y su posible aplicación operativa. |

## Uso de herramientas de IA

Durante el desarrollo se utilizaron herramientas de inteligencia artificial como apoyo para discutir alternativas metodológicas, revisar propuestas de implementación, mejorar la documentación y estructurar el proyecto.

Las decisiones relacionadas con el planteamiento del problema, selección de variables, construcción de modelos, interpretación de resultados y conclusiones finales fueron revisadas, adaptadas y validadas manualmente.