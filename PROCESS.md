# Proceso de trabajo

Este documento registra el proceso seguido durante el desarrollo de la prueba técnica.

## Enfoque inicial

Decidí abordar el problema como un caso de forecasting de demanda diaria a nivel tienda-categoría, ya que este nivel de granularidad permite generar recomendaciones accionables para la operación del negocio.

## Herramientas utilizadas

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook
- Git y GitHub
- Herramientas de AI como apoyo para estructuración del proyecto, revisión de ideas, documentación y discusión metodológica.

## Decisiones iniciales

- Variable objetivo preliminar: `total_transactions`.
- Granularidad del modelo: tienda-categoría-día.
- Validación esperada: split temporal.
- Métricas candidatas: MAE, RMSE y WAPE.