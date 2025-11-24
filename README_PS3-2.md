# PS3 — Big Data & Machine Learning para Economía Aplicada  
### Predicción del precio de vivienda en Bogotá (Grupo 10)

Este repositorio contiene el desarrollo del Problem Set 3, cuyo objetivo es construir un modelo de valoración automatizada (AVM) para predecir el precio de inmuebles en Bogotá. El proyecto combina datos de avisos inmobiliarios con información espacial de OpenStreetMap y variables extraídas del texto de los anuncios. Con esta base enriquecida se entrenan varios modelos de Machine Learning y se generan predicciones para evaluación externa (Kaggle).

## Estructura del repositorio
- **document/** — Informe final y presentaciones.  
- **scripts/** — Código en R para limpieza, geoprocesamiento, ingeniería de variables y modelado.  
- **stores/** — Modelos entrenados, datasets procesados, gráficos y archivos de predicción.  
- **raw/** — Archivos originales `train.csv` y `test.csv`.

## Flujo general del proyecto
1. Limpieza inicial y unión de bases.  
2. Enriquecimiento espacial con `sf` y datos OSM (parques, transporte, colegios, restaurantes, gimnasios).  
3. Extracción de variables desde texto (tipo de inmueble, amenidades).  
4. Construcción de la base final e imputación.  
5. Entrenamiento de múltiples modelos (regresión, regularización, árboles, bosques, boosting y ensamble).  
6. Evaluación mediante MAE y generación de archivos para Kaggle.

## Requisitos
R actualizado y paquetes como `tidyverse`, `sf`, `osmdata`, `caret`, `tidymodels`, entre otros.
