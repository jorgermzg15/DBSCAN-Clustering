# DBSCAN — Clustering Basado en Densidad

Este repositorio contiene un notebook de Jupyter que explora **DBSCAN** (Density-Based Spatial Clustering of Applications with Noise), un algoritmo de clustering que agrupa puntos cercanos entre sí y marca como outliers aquellos que se encuentran en regiones de baja densidad.

## ¿Qué es DBSCAN?

A diferencia de algoritmos como K-Means que asumen clústeres esféricos, DBSCAN puede descubrir clústeres de **formas arbitrarias** sin necesidad de especificar el número de clústeres de antemano. Se basa en dos parámetros principales:

| Parámetro | Descripción |
|-----------|-------------|
| **Epsilon (ε)** | Distancia máxima entre dos puntos para considerarse vecinos. |
| **min_samples** | Número mínimo de vecinos para que un punto sea considerado un punto central. |

## Contenido del Notebook

- Fundamentos matemáticos: distancia euclidiana, distancia de Haversine, estructuras de datos (KD-Tree, Ball-Tree).
- Efecto de la escala en el cálculo de distancias y escalado con MinMaxScaler.
- Ejemplo práctico con el dataset sintético `make_moons`.
- Comparación visual entre DBSCAN y K-Means.

## Estructura del Proyecto

```
├── DBSCAN.ipynb       # Notebook principal
├── requirements.txt   # Dependencias de Python
└── README.md
```

## Inicio Rápido con GitHub Codespaces

La forma más sencilla de ejecutar este proyecto es con GitHub Codespaces, sin instalar nada en tu máquina local.

1. En la página del repositorio, haz clic en **Code** → **Codespaces** → **Create codespace on main**.
2. Una vez que el Codespace esté listo, abre una terminal y ejecuta:
   ```bash
   pip install -r requirements.txt
   ```
3. Abre `DBSCAN.ipynb` y selecciona el kernel de Python cuando VS Code lo solicite.
4. Ejecuta las celdas en orden con **Shift + Enter**.

## Instalación Local (alternativa)

Si prefieres trabajar en tu máquina:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/jorgermzg15/aprendizaje-no-supervisado.git
   cd aprendizaje-no-supervisado
   ```

2. Crea un entorno virtual e instala las dependencias:
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # En Windows: .venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. Abre el notebook:
   ```bash
   jupyter notebook DBSCAN.ipynb
   ```

## Dependencias

- Python ≥ 3.10
- pandas, numpy, matplotlib, scikit-learn, scipy, statsmodels, plotly, ipykernel

Consulta [requirements.txt](requirements.txt) para las versiones específicas.

## Licencia

Proyecto disponible para fines educativos.
