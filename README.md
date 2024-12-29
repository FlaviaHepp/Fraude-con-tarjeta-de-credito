# Fraude-con-tarjeta-de-credito
Detección de fraudes con tarjetas de crédito (2013)

Analicé 284,807 transacciones con un 0.172% de fraudes, utilizando un pipeline de machine learning para abordar un desbalance de clases extremo.
Aplicación de técnicas como submuestreo, sobremuestreo (SMOTE) y reducción de valores atípicos para preprocesamiento de datos.
Implementé clasificadores como regresión logística, árboles de decisión, SVM y redes neuronales, logrando mejoras significativas en métricas clave de detección de fraudes.
Diseñé visualizaciones detalladas para análisis exploratorio y evaluación de modelos, como matrices de confusión, curvas ROC y gráficos de precisión/recuperación.

Este proyecto está enfocado en la detección de fraudes con tarjetas de crédito ,

**1. Contexto del proyecto**
Datos: Transacciones
Problema: D
Objetivo:Desarrollo
**2. Preprocesamiento de datos**
Ver re

Escalado de variables:

Las columnas Timey `AmAmountSí es
Manejo del desequilibrio:

Submuestreo aleatorio: Reducción de
SMOTE (Técnica de sobremuestreo de minorías sintéticas): G
Eliminación de valores atípicos:

S
División del conjunto de datos:

Los d
**3. Análisis exploratorio**
Se analizaron distribuciones de las características transformadas por PCA.
Matrices de evaluación para identificar variables clave.
Gráficos de caja para visualizar diferencias entre transacciones fraudulentas y no fraudulentas.
**4. Modelos de clasificación**
Yo si

Regresión logística:

Modelo lineal que se destacó como uno de los mejores para este problema.
Optimizado con GridSearchCVpara encontrar los mejores hiperparámetros.
Vecinos Más Cercanos (KNN):

Comparado por su simplicidad, aunque mostró limitaciones debido al tamaño y la distribución de los datos.
Máquinas de vectores de soporte (SVM):

Utilizó diferentes núcleos ( rbf, linear) para encontrar el más adecuado para este problema.
Árboles de decisión:

Modelo interpretativo y rápido, pero menos efectivo en este caso debido al desequilibrio de clases.
**5. Métricas de evaluación**
Se usaron varias métricas para evaluar el desempeño de los modelos:

Precisión: Qué tan bien el modelo clasifica correctamente.
Recuperación: Qué proporción de fraudes detecta el modelo.
F1-Score: Promedio armonizado entre precisión y recuperación.
Curva ROC: Visualización del balance entre verdaderos positivos y falsos positivos.
Curvas de Aprendizaje: Para evaluar el ajuste del modelo.
**6. Redes neuronales**
Se implementó un modelo simple con Keras:

Una capa de entrada, una capa oculta (32 neuronas) y una capa de salida.
Comparado con otros modelos usando datos balanceados con submuestreo y sobremuestreo (SMOTE).
Resultados prometedores, mostrando que la red neuronal puede clasificar fraudes con alta precisión.
**7. Resultados**
Regresión Logística: Consistentemente obtuvo las mejores métricas, especialmente en datos balanceados con SMOTE.
SVM: También mostró buenos resultados, pero con tiempos de ejecución más altos.
Redes Neuronales: Demostraron ser competitivos y capaces de detectar fraudes de manera precisa.
Conclusiones
Mejor Modelo: La Regresión Logística con SMOTE se destacó como el modelo más efectivo para este conjunto de datos.
Importancia del Preprocesamiento: Técnicas como SMOTE y la eliminación de valores atípicos mejoraron significativamente los resultados.
Equilibrio entre precisión y recuperación: Es crucial en problemas como este para evitar errores incorrectos que puedan afectar a los clientes.
