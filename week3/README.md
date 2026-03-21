## Actividad 2 Semana 3
> **Tarea:**  Implementar y validar el proceso de aprendizaje de una red neuronal mediante backpropagation y el uso de funciones de activación.

> [!TIP]
> **Solución Actividad 2:** Codigo ejecutado en Google Colab y exportado en formato .ipynb (week3/Actividad2.ipynb) con el analisis de la realizacion de una Red Neuronal con Aprendizaje Backpropagation y Funciones de Activación en anotaciones (Markdown).

Para este algoritmo se agregaron dos entradas X1, X2, cuatro capas ocultas H1, H2, H3, H4 y una salida. Los datos de entrada y etiquetas se generan una unica vez desde un dataset de numpy. Este modelo se empleo igual para las dos funciones de activacion y asi poder realizar una comparacion valida.

Dataset ──► Forward Pass ──► Predicción ──► Cálculo de error ──► Backpropagation ──► Ajuste de pesos ──► Repetir 2000 veces ──► Modelo entrenado

El gran análisis de este ejercicio es que la red neuronal logra reducir el error durante el entrenamiento, lo que indica que está aprendiendo. Esto es evidenciable en los resultados por cada Epoca el error disminuye progresivamente, demostrando que el algoritmo de backpropagation y descenso de gradiente funciona correctamente.

Tambien es evidenciable como los pesos iniciales son muy diferentes a los finales, demostrando que el algoritmo se adapta para optimizar la salida.

En cuanto a la comparación de las funciones de activación Sigmoid y ReLu se puede mencionar que la eleccion de una función de activación influye en el desempeño del modelo. Aquí se puede observar que ReLU suele presentar una convergencia más rápida y con mayor precisión que Sigmoid

<sub>Autor: Jhoan Avila Gutierrez<sub>
