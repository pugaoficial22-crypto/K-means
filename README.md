K-means (housing.csv)
```markdown
# Clustering K-means – Segmentación de viviendas en California

Autor: Diego Ivan Prieto Puga  
Fecha: 11 Diciembre 2025

## Objetivo
Segmentar las viviendas del dataset California Housing mediante **K-means** y encontrar el número óptimo de clusters con el método del codo y silhouette score.

## Archivos
- Clustering_Housing.ipynb → Todo el proceso + visualización 2D con PCA
- housing.csv → Dataset completo
- kmeans_housing_model.pkl → Modelo K-means entrenado (K = X)
- scaler_housing.pkl → StandardScaler usado (necesario para nuevas predicciones)
- requirements.txt

## Resultados
- K óptimo seleccionado: X
- Silhouette Score: 0.XX
- Inertia final: XXX,XXX
- Visualización clara de los clusters geográficos y socioeconómicos

## Uso
```python
import joblib
kmeans = joblib.load('Diego_clustering_housing.pkl')
scaler = joblib.load('scaler_housing.pkl')
cluster = kmeans.predict(scaler.transform(nueva_vivienda))
