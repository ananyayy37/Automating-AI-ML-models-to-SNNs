# ANN to SNN Conversion using NengoDL

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-FF6F00?logo=tensorflow&logoColor=white)
![NengoDL](https://img.shields.io/badge/NengoDL-SNN-green)
![MNIST](https://img.shields.io/badge/Dataset-MNIST-blue)

This repository contains two implementations of Spiking Neural Networks (SNNs) on the MNIST dataset:

- ANN to SNN conversion using **NengoDL**
- Direct SNN training using **surrogate gradient backpropagation**

---

## Features

- Train a LeNet-5 CNN on the MNIST dataset
- Convert a trained ANN into an SNN using NengoDL
- Replace ReLU activations with Leaky Integrate-and-Fire (LIF) neurons
- Perform spike-based inference over multiple timesteps
- Train an SNN directly using surrogate gradient backpropagation

---

## ANN to SNN Conversion Pipeline

```text
MNIST
   │
   ▼
Train ANN
   │
   ▼
Convert using NengoDL
   │
   ▼
Replace ReLU with LIF Neurons
   │
   ▼
Run SNN for Multiple Timesteps
   │
   ▼
Prediction
```

---

## Leaky Integrate-and-Fire (LIF) Neuron

An LIF neuron accumulates incoming spikes in its membrane potential. When the membrane potential reaches a threshold, the neuron emits a spike and the membrane potential is reset.


---

## Repository Contents

### `ANN_to_SNN_Conversion.ipynb`

- Train a LeNet-5 ANN on MNIST
- Convert the trained ANN to an SNN using NengoDL
- Perform spike-based inference

### `Direct_SNN_Training.ipynb`

- Train an SNN directly using surrogate gradient backpropagation
- Use Poisson spike encoding
- Implement custom LIF neurons
- Train using TensorFlow

### `Presentation.pdf`

Project presentation describing the implementation and concepts used.

---

## Technologies Used

- Python
- TensorFlow / Keras
- Nengo
- NengoDL
- NumPy
- Matplotlib

---

## Installation

```bash
git clone https://github.com/<username>/<repository-name>.git

cd <repository-name>

pip install -r requirements.txt
```

---

## References

- TensorFlow
- Nengo
- NengoDL
