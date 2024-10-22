# Análisis de predicción del desempeño académico basado en Factores Estudiantiles

## Descripción del Proyecto

Este proyecto tiene como objetivo predecir el puntaje de los exámenes de los estudiantes, basándonos en diversas características relacionadas con el entorno académico y familiar, actividades extracurriculares, e influencias sociales. Se trabajó con modelos de machine learning para entender cómo distintos factores impactan en el rendimiento académico.

## Pasos Realizados

### 1. Exploración y Limpieza de Datos

Antes de comenzar con el modelado, se realizó un análisis exhaustivo de los datos. Este proceso incluyó:

-   **Análisis de valores nulos**: Se identificaron y reemplazaron valores faltantes en el conjunto de datos, utilizando estrategias como la imputación de la media para datos numéricos y la moda para los categóricos.
-   **Identificación de valores atípicos (outliers)**: Se identificaron los valores extremos en las variables utilizando el método del rango intercuartílico (IQR), y se tomaron decisiones para ajustarlos y evitar que afecten a los modelos.

### 2. Análisis Exploratorio de Datos

Durante esta fase, se realizaron varias comparaciones entre las variables, buscando relaciones importantes que podrían ser útiles para el modelo predictivo. Este análisis incluyó:

-   Comparación de variables numéricas y categóricas.
-   Visualización de tendencias mediante gráficos de barras, gráficos de dispersión y boxplots.
-   Evaluación del impacto de diferentes características (como la calidad del maestro, el nivel de involucramiento parental, etc.) sobre el rendimiento académico.

### 3. Modelado Predictivo

Se aplicaron diversos modelos de regresión para predecir el puntaje de exámenes. Estos modelos fueron entrenados y probados con un conjunto de datos separado para evaluar su rendimiento. Los modelos utilizados fueron:

-   **Regresión Lineal**
-   **Regresión Ridge**
-   **Regresión Lasso**
-   **Random Forest**
-   **Árbol de Decisión**

Además, se utilizó un modelo avanzado de **Stacking Regressor**, que combina la fuerza de múltiples modelos para mejorar la precisión.

### 4. Evaluación de los Modelos

Se utilizaron varias métricas de evaluación para comparar el desempeño de los modelos:

-   **Error Absoluto Medio (MAE)**: Mide el error promedio entre las predicciones y los valores reales.
-   **Raíz del Error Cuadrático Medio (RMSE)**: Penaliza los errores más grandes y da una visión clara de la precisión del modelo.
-   **Coeficiente de Determinación (R²)**: Indica qué porcentaje de la variabilidad de los puntajes de examen es explicada por el modelo.

### 5. Resultados Finales

Los resultados demostraron que el modelo **Stacking Regressor** fue el más preciso para predecir los puntajes de examen:

-   **Sin Datos Atípicos**:
    
    -   **MAE**: 0.8760
    -   **RMSE**: 1.2578
    -   **R²**: 0.8588
    
    Esto significa que el modelo fue capaz de explicar más del 85% de la variabilidad en los puntajes de examen, con un bajo error en las predicciones.
    
-   **Con Datos Atípicos**:
    
    -   **MAE**: 0.9709
    -   **RMSE**: 1.9767
    -   **R²**: 0.7131
    
    Aunque los resultados son aceptables, la presencia de outliers afectó la precisión del modelo, reforzando la importancia de ajustar los valores atípicos.
    

### 6. Conclusión

El proyecto mostró que factores como el nivel de involucramiento parental, las actividades extracurriculares y el acceso a recursos educativos son elementos clave en el rendimiento académico de los estudiantes. Además, el preprocesamiento adecuado de los datos (como el tratamiento de valores atípicos) mejora considerablemente el rendimiento de los modelos predictivos.

El modelo **Stacking Regressor** se destacó como la mejor opción para esta tarea, mostrando gran precisión en la predicción de los puntajes de examen.

### Herramientas utilizadas
- Vscode
- Quarto
- Kaggle

## Contacto

- **Nombre:** Leandro Soto Miranda
- **Correo Electrónico:** [lea](mailto:leasotompriv@gmail.com)
- **LinkedIn:** [LinkedIn](https://www.linkedin.com/in/leandro-soto-miranda-767a72264/)