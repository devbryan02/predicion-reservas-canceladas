# Hotel Bookings Big Data

Proyecto de análisis y modelado sobre el dataset de reservas de hotel `hotel_bookings`.
El objetivo es recorrer todo el flujo de datos: ingesta, persistencia en SQL y MongoDB,
análisis exploratorio, entrenamiento de un modelo predictivo y generación de resultados.

## Qué contiene el proyecto

- `data/`: datos originales, datos imputados y exportaciones para MongoDB.
- `db/`: base de datos SQLite local usada en la parte relacional.
- `models/`: modelo entrenado y serializado.
- `notebooks/`: desarrollo paso a paso del proceso completo.
- `reports/`: visualizaciones y entregables generados durante el análisis.

## Flujo de trabajo

1. `01_Ingesta_y_SQL.ipynb`: carga de datos y preparación de la base relacional.
2. `02_NoSQL_y_MongoDB.ipynb`: exportación y trabajo con MongoDB.
3. `03_EDA_y_Visualizacion.ipynb`: análisis exploratorio y gráficos principales.
4. `04_Machine_Learning.ipynb`: entrenamiento y evaluación del modelo.
5. `05_Predict_Model.ipynb`: uso del modelo para hacer predicciones.

## Datos incluidos

- `data/hotel_bookings.csv`: dataset original.
- `data/hotel_bookings_imputed.csv`: versión con imputación de valores faltantes.
- `data/mongo_export.json`: exportación para MongoDB.
- `data/mongo_clients_new.json`: clientes o registros preparados para MongoDB.

## Resultados y artefactos

- `db/hotel_local.db`: base SQLite local.
- `models/random_forest_cancelaciones.pkl`: modelo guardado.
- `reports/*.png`: gráficos y resúmenes visuales del análisis.

## Requisitos

El proyecto usa Python y las siguientes librerías principales:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `sqlalchemy`
- `pymongo`
- `dnspython`

Instalación:

```bash
pip install -r requirements.txt
```

## Cómo usarlo

1. Instala las dependencias.
2. Abre los notebooks en orden dentro de `notebooks/`.
3. Revisa los datos en `data/` y los resultados generados en `reports/` y `models/`.

## Objetivo del análisis

El foco del proyecto es estudiar el comportamiento de las reservas de hotel y construir un modelo que ayude a estimar cancelaciones u otros patrones relevantes del dataset.
