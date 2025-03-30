# Aprendizaje por Refuerzo I - Trabajos Prácticos

Este repositorio contiene los trabajos prácticos de la materia **Aprendizaje por Refuerzo I** de la **Maestría en Inteligencia Artificial** de la **Facultad de Ingeniería de la Universidad de Buenos Aires (FIUBA)**.

## Integrantes

- **Juan Ignacio Ribet**\
  **N° SIU:** a1001
- **Fabian Sarmiento**\
  **N° SIU:** 2672002

## Trabajos Prácticos

1. **TP1: Q-Learning**\
   Implementación de la estrategia de aprendizaje por refuerzo basada en **Q-Learning** para resolver un entorno de toma de decisiones discreto.

2. **TP2: Deep Q-Learning**\
   Extensión del Q-Learning utilizando redes neuronales profundas (**Deep Q-Networks - DQN**) para mejorar la capacidad de generalización en entornos complejos y de alta dimensionalidad.

3. **TP3: Actor-Critic**\
   Implementación del método **Actor-Critic**, una técnica de aprendizaje por refuerzo basada en políticas que combina un actor (que toma decisiones) y un crítico (que evalúa las decisiones tomadas).

## Estructura del Repositorio

```
Aprendizaje-Por-Refuerzo-I
│── tp1_q_learning
│   ├── README.md
│   ├── mountain_car.pkl
│   ├── mountain_car_metrics.csv
│   ├── mountain_car_p_learning.ipynb
│   ├── mountain_car_training_results.png
│   ├── training_results/
│   │   ├── mountain_car_metrics_20250321_222356.csv
│   │   ├── training_params_20250321_222356.txt
│── tp2_deep_q_learning
│   ├── README.md
│── tp3_actor_critic
│   ├── README.md
│── requirements.txt
│── README.md
```

## Instalación y Uso

Para ejecutar los trabajos prácticos, es recomendable crear un entorno virtual y luego instalar las dependencias necesarias:

```sh
python -m venv venv
source venv/bin/activate  # En Windows: venv\Scripts\activate
pip install -r requirements.txt
```

Cada trabajo práctico cuenta con su propio **README.md**
