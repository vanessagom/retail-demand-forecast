# Retail Demand Forecast

## Descripción

Este proyecto desarrolla una solución de *forecasting* para estimar la demanda diaria a nivel **tienda–categoría**, utilizando información histórica de transacciones, características de tiendas y variables de calendario.

El objetivo es generar pronósticos que apoyen la toma de decisiones relacionadas con inventario, personal operativo y planificación de promociones.

## Objetivo

Construir un modelo capaz de predecir el número diario de transacciones para cada combinación de tienda y categoría, manteniendo un enfoque orientado al negocio y a la posible automatización del proceso de predicción.

## Estructura del proyecto

```text
retail-demand-forecast/
├── data/
│   ├── raw/
│   └── processed/
├── figures/
├── notebooks/
│   ├── explore_analysis.ipynb
│   └── train_forecast_model.ipynb
├── outputs/
├── src/
│   ├── data_preparation.py
│   ├── feature_engineering.py
│   ├── train_model.py
│   ├── evaluate.py
│   └── predict.py
├── .gitignore
├── PROCESS.md
├── README.md
└── requirements.txt