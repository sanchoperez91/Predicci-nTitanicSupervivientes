# 🛳 Titanic Survival Prediction Project

Este proyecto utiliza un modelo de Machine Learning para predecir qué pasajeros del Titanic tenían más probabilidades de sobrevivir al naufragio. Es parte de un ejercicio grupal en el que aplicamos conceptos de análisis de datos y técnicas de Machine Learning.

## 📁 Descripción del Proyecto

### Objetivo
Crear un modelo predictivo para determinar la probabilidad de supervivencia de los pasajeros del Titanic en función de características como la clase de boleto, el género y la cantidad de acompañantes.

### Dataset
El conjunto de datos de entrenamiento incluye información de los pasajeros, como:
- **Pclass**: Clase de boleto (1, 2, o 3)
- **Sex**: Género del pasajero
- **SibSp**: Número de hermanos/esposas a bordo
- **Parch**: Número de padres/hijos a bordo
- **Fare**: Tarifa del boleto
- **Age**: Edad del pasajero (algunos valores faltantes)

## 🛠 Técnicas y Modelos Utilizados

Para este proyecto, utilizamos:
- **Librerías**: `Pandas` para manejo de datos, `NumPy` para álgebra lineal y `RandomForestClassifier` de `sklearn.ensemble` como modelo.
- **Modelo de Machine Learning**: `RandomForestClassifier` con 100 árboles y una profundidad máxima de 5 para balancear precisión y simplicidad del modelo.

## 🔍 Análisis y Resultados

### Análisis Exploratorio
- **Distribución por Género y Supervivencia**: Observamos que el porcentaje de mujeres sobrevivientes fue significativamente mayor que el de hombres.
- **Impacto de la Clase de Boleto**: Las clases más altas tienen mayores tasas de supervivencia.

### Resultados del Modelo
El modelo final se entrenó con los datos preprocesados usando las siguientes características:
- **Características**: `Pclass`, `Sex`, `SibSp`, y `Parch`
- **Evaluación Inicial**: Comparamos las tasas de supervivencia por género y observamos que el modelo capturaba patrones similares.

## ⚙️ Ejecución del Código

Para ejecutar el código, sigue estos pasos:

1. Descarga el conjunto de datos de [Kaggle](https://www.kaggle.com/competitions/titanic) y colócalo en la carpeta correspondiente.
2. Corre el script `python titanic_prediction.py` desde tu entorno de desarrollo.
3. El script generará un archivo `submission.csv` con las predicciones para enviar a Kaggle.

```python
# Ejemplo de ejecución en Python
python titanic_prediction.py

