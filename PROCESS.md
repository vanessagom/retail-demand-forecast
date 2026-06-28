# PROCESS

## Objetivo

Documentar el proceso seguido durante el desarrollo del proyecto, incluyendo metodología, herramientas utilizadas y decisiones técnicas principales.

## Enfoque del proyecto

El proyecto se aborda como un problema de forecasting de demanda diaria a nivel tienda-categoría. Este nivel de granularidad permite generar predicciones más accionables para apoyar decisiones de inventario, asignación de personal y planeación promocional.

## Metodología

El flujo de trabajo seguirá las siguientes etapas:

1. Comprensión del problema de negocio.
2. Carga y validación inicial de datos.
3. Análisis exploratorio.
4. Evaluación de calidad de datos.
5. Ingeniería de variables.
6. Desarrollo de modelos de forecasting.
7. Evaluación del desempeño.
8. Generación de predicciones y recomendaciones de negocio.

## Estructura técnica

El proyecto combinará notebooks y scripts de Python:

- Los notebooks se utilizarán para análisis exploratorio, visualización, justificación metodológica e interpretación de resultados.
- Los scripts dentro de `src/` concentrarán código modular y reutilizable, con el objetivo de acercar el proyecto a un flujo reproducible y potencialmente automatizable.

## Registro de decisiones

Esta sección se actualizará conforme avance el proyecto.

| Decisión | Justificación |
|---|---|
| Modelar la demanda a nivel tienda-categoría | Permite generar predicciones accionables para decisiones operativas más específicas. |
| Utilizar `total_transactions` como variable objetivo inicial | Representa una aproximación directa a la demanda operativa y al flujo esperado de clientes. |
| Mantener notebooks y scripts separados | Los notebooks permiten documentar el análisis; los scripts facilitan reproducibilidad y automatización. |

## Uso de herramientas de AI

Durante el desarrollo se utilizaron herramientas de inteligencia artificial como apoyo para discutir alternativas metodológicas, estructurar documentación, revisar ideas de implementación y mejorar la claridad de las explicaciones.

Todas las decisiones técnicas, interpretación de resultados y adaptación del enfoque fueron revisadas manualmente.