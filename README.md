# Descripción

Este código es una implementación de un modelo de clasificación utilizando el algoritmo Naive Bayes con dos variantes: MultinomialNB y GaussianNB. El objetivo principal es clasificar datos de diagnóstico médico en diferentes categorías de pronóstico. Para lograr esto, se utiliza un conjunto de datos previamente dividido en conjuntos de entrenamiento y prueba.
Fue realizado para la Universidad Politécnica de Varsovia. Asignatura de Inteligencia Artificial

# Librerías utilizadas

pandas: Utilizada para la manipulación y análisis de datos en forma de tablas.
matplotlib.pyplot: Usada para la visualización de gráficos y diagramas.
seaborn: Utilizada para mejorar y personalizar la visualización de los mapas de calor (heatmaps).
sklearn.naive_bayes.MultinomialNB: Implementación del algoritmo de Naive Bayes para datos discretos.
sklearn.naive_bayes.GaussianNB: Implementación del algoritmo de Naive Bayes para datos continuos.
time: Utilizada para medir el tiempo de ejecución del código.
joblib: Usada para guardar y cargar modelos entrenados.
eli5: Utilizada para explicar y visualizar el funcionamiento de modelos de machine learning.
eli5.sklearn.PermutationImportance: Empleada para calcular la importancia de las características mediante la permutación de sus valores.
sklearn.metrics: Contiene funciones para calcular métricas de evaluación de modelos, como precisión, recall, matriz de confusión, etc.
Datos

El conjunto de datos se carga desde dos archivos CSV: "Training.csv" y "Testing.csv". El archivo "Training.csv" se utiliza para entrenar el modelo y el archivo "Testing.csv" se emplea para evaluar el rendimiento del modelo.

# Preparación de los datos

Se separan las características (X) de las etiquetas de clasificación (Y) tanto para el conjunto de entrenamiento como para el conjunto de prueba. Las características de entrenamiento se almacenan en "X_train", las etiquetas de entrenamiento en "Y_train", las características de prueba en "X_test" y las etiquetas de prueba en "Y_test".

# Entrenamiento y Evaluación del Modelo

Se entrena el modelo de Naive Bayes Multinomial y el modelo de Naive Bayes Gaussiano utilizando los datos de entrenamiento. Luego, se realiza una predicción en el conjunto de prueba y se evalúa el rendimiento del modelo mediante la precisión (accuracy), la matriz de confusión y el informe de clasificación.

# Visualización de la Matriz de Confusión

Se crea un mapa de calor (heatmap) de la matriz de confusión para visualizar de manera más clara la precisión de las predicciones del modelo.

# Resultados

El modelo muestra una precisión del 100% en el conjunto de prueba ("Testing.csv"). Sin embargo, es importante tener en cuenta que un rendimiento perfecto en el conjunto de prueba puede ser indicativo de un posible sobreajuste del modelo a los datos de entrenamiento. Es recomendable realizar pruebas adicionales y validar el rendimiento del modelo con nuevos conjuntos de datos antes de considerarlo completamente válido.
