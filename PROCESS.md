# PROCESS

## Objetivo

Documentar el proceso seguido durante el desarrollo del proyecto, incluyendo la metodología aplicada, las herramientas utilizadas y las principales decisiones técnicas tomadas durante la construcción del modelo de forecasting.

## Enfoque del proyecto

El proyecto se aborda como un problema de forecasting de demanda diaria a nivel **tienda–categoría**. Este nivel de granularidad permite generar predicciones más accionables para apoyar decisiones relacionadas con inventario, asignación de personal, abastecimiento y planeación promocional.

El desarrollo sigue un enfoque iterativo, donde las decisiones de modelado se sustentan en evidencia obtenida durante el análisis exploratorio y en la evaluación continua del desempeño de los modelos.

## Metodología

El flujo de trabajo siguió las siguientes etapas:

1. Comprensión del problema de negocio.
2. Carga y validación inicial de datos.
3. Análisis exploratorio de datos (EDA).
4. Evaluación de calidad de datos.
5. Ingeniería de variables.
6. Desarrollo y comparación de modelos de forecasting.
7. Interpretación del modelo y análisis de importancia de variables.
8. Evaluación del desempeño sobre datos no observados.
9. Construcción de un caso de uso orientado al negocio.

## Estructura técnica

El proyecto combina notebooks y scripts de Python con objetivos distintos:

- Los notebooks documentan el análisis exploratorio, la justificación metodológica, el desarrollo de modelos y la interpretación de resultados.
- Los scripts dentro de `src/` concentrarán código modular y reutilizable, buscando facilitar la reproducibilidad y una futura automatización del proyecto.

## Registro de decisiones

Esta sección se actualizará conforme avance el proyecto.

| Decisión | Justificación |
|---|---|
| Modelar la demanda a nivel tienda–categoría | Permite generar predicciones accionables para decisiones operativas más específicas. |
| Utilizar `total_transactions` como variable objetivo inicial | Representa una aproximación directa a la demanda operativa y al flujo esperado de clientes. |
| Excluir variables que no estarán disponibles al momento de predecir (por ejemplo `replenishment_signal`) | Evita fuga de información (*data leakage*) y garantiza un escenario de predicción realista. |
| Utilizar un baseline antes de modelos más complejos | Permite medir si los modelos de Machine Learning realmente aportan valor adicional. |
| Mantener notebooks y scripts separados | Los notebooks documentan el análisis; los scripts facilitan reproducibilidad y automatización. |
| Evaluar distintos esquemas de validación temporal | En forecasting, el diseño del split puede influir significativamente en la evaluación del modelo y debe validarse explícitamente. |

## Uso de herramientas de IA

Durante el desarrollo se utilizaron herramientas de inteligencia artificial como apoyo para discutir alternativas metodológicas, estructurar documentación, revisar propuestas de implementación y mejorar la claridad de las explicaciones.

Todas las decisiones relacionadas con el enfoque metodológico, selección de variables, interpretación de resultados y conclusiones finales fueron revisadas y adaptadas por mí la autora Vanessa Gómez.
