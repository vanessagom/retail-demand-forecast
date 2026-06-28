# Retail Demand Forecast

## Descripción

Este proyecto desarrolla una solución de *forecasting* para estimar la demanda diaria a nivel **tienda–categoría**, utilizando información histórica de transacciones, características de tiendas y variables de calendario.

El objetivo es generar pronósticos que apoyen la toma de decisiones relacionadas con inventario, personal operativo y planificación de promociones.

## Objetivo

Construir un modelo capaz de predecir el número diario de transacciones para cada combinación de tienda y categoría, manteniendo un enfoque orientado al negocio y a la posible automatización del proceso de predicción.

## Estructura del proyecto

```
retail-demand-forecast/
│
├── data/
│   ├── processed/
│   └── raw/
│       ├── calendar.csv
│       ├── stores.csv
│       └── transactions.csv
│
├── notebooks/
│   ├── explore_analysis.ipynb
│   └── train_forecast_model.ipynb
│
├── outputs/
│
├── .gitignore
├── PROCESS.md
└── README.md
```

## Contenido

### 1. Análisis exploratorio
- Calidad de los datos
- Comportamiento temporal de la demanda
- Estacionalidad
- Promociones y eventos comerciales
- Formato de tienda
- Diferencias regionales
- Principales hallazgos de negocio

### 2. Modelo de forecasting
- Construcción del dataset de modelado
- Ingeniería de variables
- División temporal de entrenamiento, validación y prueba
- Modelo baseline
- Regresión lineal
- LightGBM
- Interpretación del modelo
- Evaluación final
- Caso de uso para negocio

## Modelos evaluados

- Baseline (Lag 7)
- Regresión Lineal
- LightGBM

## Métricas de evaluación

- MAE
- RMSE
- MAPE
- WAPE
- R²

