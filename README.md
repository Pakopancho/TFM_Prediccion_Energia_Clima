# Predicción de la Demanda Eléctrica mediante Machine Learning y Deep Learning

## Descripción

Este repositorio contiene el código fuente, los datos y los materiales desarrollados para el Trabajo Fin de Máster titulado:

**Analisis predictivo del consumo eléctrico mediante datos meteorológicos abiertos**

El proyecto desarrolla un flujo completo de análisis siguiendo la metodología CRISP-DM, incluyendo la preparación de los datos, el entrenamiento de modelos predictivos, la evaluación de resultados y la creación de un dashboard interactivo en Power BI.

---

## Objetivos

- Integrar datos de demanda eléctrica y variables meteorológicas.
- Analizar el comportamiento temporal de la demanda.
- Implementar modelos baseline (Regresión Lineal y Random Forest).
- Desarrollar modelos LSTM univariante y multivariante.
- Comparar el rendimiento de todos los modelos mediante las métricas MAE, RMSE y MAPE.
- Visualizar los resultados mediante un dashboard interactivo en Power BI.

---

## Estructura del repositorio

```text
TFM_Nombre_Apellido/

├── datos/
│   ├── dataset_energia_clima_limpio.csv
│   ├── energy_dataset.csv
│   └── weather_features.csv
│
├── resultados/
│   ├── dashboard_powerbi.csv
│   ├── history_multi.csv
│   ├── history_uni.csv
│   ├── importancia_caracteristicas.csv
│   ├── metricas_modelos.csv
│   └── resultados_optimizacion_hiperparametros.csv
│
├── dashboard/
│   └── Dashboard_TFM.pbix
│
├── Desarrollo_TFM.ipynb
├── TFM_Jose_Sanchez_Final.pdf
├── README.md
└── .gitignore
```

---

## Requisitos

- Python 3.11 o superior

Principales librerías utilizadas:

- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- tensorflow
- keras

---

## Ejecución

1. Clonar el repositorio.

2. Instalar las dependencias.

3. Ejecutar el notebook:

```
Desarrollo_TFM.ipynb
```

El notebook reproduce todo el flujo del proyecto:

- carga de datos;
- limpieza y preprocesamiento;
- análisis exploratorio;
- entrenamiento de modelos;
- optimización de hiperparámetros;
- evaluación mediante MAE, RMSE y MAPE;
- generación automática de los archivos utilizados por Power BI.

---

## Dashboard

El archivo

```
dashboard/Dashboard_TFM.pbix
```

permite explorar de forma interactiva:

- demanda real frente a demanda estimada;
- perfil horario de consumo;
- consumo por día de la semana;
- influencia de la temperatura;
- principales indicadores del modelo.

---

## Reproducibilidad

El entrenamiento de las redes LSTM incorpora procesos estocásticos derivados de la inicialización aleatoria de pesos y del algoritmo de optimización empleado.

Por este motivo, pequeñas variaciones en las métricas pueden aparecer entre ejecuciones independientes. Se ha establecido una semilla aleatoria para mejorar la reproducibilidad del proceso experimental.

---

## Autor

José Sánchez

Trabajo Fin de Máster

Máster Universitario en Análisis y Visualización de Datos Masivos/ Visual Analytics and Big Data

Universidad Internacional de La Rioja
Escuela Superior de Ingeniería y Tecnología

2026