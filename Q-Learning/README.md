# Proyecto de Aprendizaje por Refuerzo: MountainCar

Este proyecto implementa el algoritmo de Q-learning para resolver el problema clásico de control conocido como MountainCar. El objetivo es que un coche aprenda a subir una colina empinada utilizando aprendizaje por refuerzo.

## Descripción del Problema

En el entorno de MountainCar, un coche se encuentra en un valle y debe aprender a ganar suficiente impulso para subir una colina. El coche puede acelerar hacia la izquierda, hacia la derecha o no acelerar. El objetivo es alcanzar la cima de la colina en el menor número de pasos posible.

## Algoritmo de Q-learning

Q-learning es un algoritmo de aprendizaje por refuerzo que busca encontrar la política óptima para un problema de decisión secuencial. Se basa en la función de valor Q, \( Q(s, a) \), que estima la utilidad de tomar una acción \( a \) en un estado \( s \). La función Q se actualiza iterativamente usando la ecuación de Bellman:

\[
Q(s, a) \leftarrow Q(s, a) + \alpha \left[ r + \gamma \max_{a'} Q(s', a') - Q(s, a) \right]
\]

Donde:
- \( \alpha \) es la tasa de aprendizaje.
- \( r \) es la recompensa recibida.
- \( \gamma \) es el factor de descuento.
- \( s' \) es el nuevo estado.

## Aplicación en MountainCar

El agente utiliza Q-learning para aprender la mejor secuencia de acciones que maximicen la recompensa. La política se deriva de la función Q, eligiendo la acción con el valor Q más alto en cada estado. Se utiliza una estrategia \(\epsilon\)-greedy para equilibrar la exploración y la explotación.

## Resultados

Los resultados del entrenamiento se pueden encontrar en el archivo `mountain_car_metrics.csv` y se visualizan en `mountain_car_training_results.png`. Estos muestran cómo el agente mejora su desempeño a lo largo del tiempo.

## Requisitos

Para ejecutar este proyecto, se requiere tener instalado Python y las bibliotecas necesarias que se pueden encontrar en el archivo `requirements.txt` (si existiera).

## Ejecución

Para ejecutar el proyecto, simplemente abra y ejecute el notebook `mountain_car_p_learning.ipynb` en un entorno compatible con Jupyter.

---

Este README proporciona una visión general del proyecto y cómo se implementa el algoritmo de Q-learning para resolver el problema de MountainCar. Para más detalles, consulte el código fuente y los comentarios en el notebook.