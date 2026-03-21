## Actividad 3 Semana 4
> **Tarea:**  Implementar y validar el proceso de aprendizaje de una red neuronal mediante hiperparámetros de entrenamiento (como tasa de aprendizaje) y optimizadores (por ejemplo, variantes de descenso por gradiente).

> [!TIP]
> **Solución Actividad 3:** Codigo ejecutado en Google Colab y exportado en formato .ipynb (week4/Actividad3.ipynb) con el analisis de la realizacion de una Red Neuronal con Tecnicas de Optimización en el aprendizaje en anotaciones (Markdown).

Para este algoritmo se agregaron dos entradas X1, X2, cuatro capas ocultas H1, H2, H3, H4 y una salida. Los datos de entrada y etiquetas se generan una unica vez desde un dataset de numpy. Este modelo emplea la funcion de activación ReLu y los mismos datos de entrada para cada optimizador para asi poder realizar una comparacion valida.

Dataset ──► Forward Pass ──► Predicción ──► Cálculo de error ──► Backpropagation ──► Ajuste de pesos con Optimizadores (SGD / SGD+LRDecay / Adam) ──► Repetir 2000 veces ──► Modelo entrenado

De acuerdo a esto y realizando un analizis de comparación se puede concluir que:
- El optimizador Adam demostró ser el más eficiente, logrando una convergencia más rápida y estable, alcanzando valores bajos de pérdida en menos épocas en comparación con SGD.
- El optimizador Learning Rate Decay presentó un rapido aprendizaje más lento, pero una pérdida mayor en etapas avanzadas del entrenamiento debido a una reducción prematura de la tasa de aprendizaje, lo que limitó la capacidad del modelo para seguir ajustando los pesos.
- El optimizador Gradiante SGB mantuvo una tasa constante que permitió mejorar la estabilidad pero redujo la capacidad de aprendizaje en etapas avanzadas.

Esto evidencia la importancia de seleccionar adecuadamente el optimizador y ajustar los hiperparámetros según el problema.

<sub>Autor: Jhoan Avila Gutierrez<sub>
