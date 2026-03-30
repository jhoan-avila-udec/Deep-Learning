## Actividad 4 Semana 4
> **Tarea:**  Aplicar métodos de regularización en una red neuronal para reducir el sobreajuste (overfitting) y mejorar la capacidad de generalización del modelo.

> [!TIP]
> **Solución Actividad 4:** Codigo ejecutado en Google Colab y exportado en formato .ipynb (week4-regularizacion/Actividad4.ipynb) con el analisis de la realizacion de una Red Neuronal con Tecnicas de Regularización en el aprendizaje en anotaciones (Markdown).

Para este algoritmo se agregaron dos entradas X1, X2, cuatro capas ocultas H1, H2, H3, H4 y una salida. Los datos de entrada y etiquetas se generan una unica vez desde un dataset de numpy.
Este modelo emplea la funcion de activación ReLu, el optimizador Gradiante SGD y los mismos datos de entrada para cada regularización (con o sin L2) para asi poder realizar una comparacion valida.

Dataset ──► Forward Pass ──► Predicción ──► Cálculo de error (regularización L2) ──► Backpropagation (regularización L2 en gradiantes) ──► Ajuste de pesos con Optimizadores (SGD) ──► Repetir 2000 veces ──► Modelo entrenado

De acuerdo a esto y realizando un analisis de comparación se puede concluir que:
- El **uso de regularización L2** reduce el overfitting y hace el entrenamiento más estable, limitando el crecimiento de los pesos y mejorando la capacidad de generalización del modelo.
- El parámetro λ en la regularización L2 controla la intensidad de la penalización sobre los pesos del modelo. En este codigo se probaron diferentes valores (por ejemplo 0.1, 0.001 y 1) concluyendo que valores excesivos pueden provocar underfitting.
- El **NO uso de regularización L2** permite que los pesos crezcan libremente, lo que mejora el ajuste a los datos de entrenamiento, pero aumenta el riesgo de capturar ruido y reducir el desempeño en datos de prueba.

Esto evidencia la importancia de aplicar una tecnica de regularización y ajustar los hiperparámetros λ adecuadamente según el problema.

***Nota:** Para ajustar a gusto el valor de λ en el codigo verifique la variable "regularizacion_lambda_L2".*

<sub>Autor: Jhoan Avila Gutierrez<sub>
