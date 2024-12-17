# Spiking Neural Network Simulations and Decoding

This repository contains simulations and experiments involving spiking neural networks (SNNs), specifically:

1. **Synfire Chain Dynamics Simulation**
2. **Neural Decoding of Motor Signals**

The project aims to model and analyse neural phenomena using leaky integrate-and-fire (LIF) models with realistic background noise and decode motor signals from neural recordings.

---

## Project Overview

### 1. Synfire Chain Dynamics Simulation

- **Objective**: Reproduce and extend the results of [Diesmann et al. (1999)](https://www.nature.com/articles/990101) on stable propagation of synchronous spikes in a neural network.
- **Methods**:
  - Leaky integrate-and-fire neuron model with **alpha synapses**.
  - Poisson background noise to simulate realistic neural activity.
  - Refractoriness to model the neuron reset state after a spike.
  - All-to-all connectivity with a fixed delay between layers.

- **Key Features**:
  - Simulation of spike bursts propagating through a layered neural network.
  - Implementation of biologically inspired **Poisson noise** and refractoriness.


---

### 2. Neural Decoding of Motor Signals

- **Objective**: Decode pointer velocity from spike trains recorded in the motor cortex.
- **Data**: Neural recordings of spike trains and corresponding movement velocities from a monkey performing a screen-pointer task.

- **Approach**:
  - A network of **leaky integrate-and-fire (LIF) neurons** processes recorded spike trains.
  - Training uses **surrogate gradient descent** to decode the velocity signals.

- **Key Components**:
  - Input spike trains and velocity signals.
  - Conversion of spike trains into meaningful predictions of pointer velocities.

- **Inspired By**:
  - ["Machine Learning for Neural Decoding" (Glaser et al. 2020)](https://doi.org/10.1523/ENEURO.0506-19.2020).

---

## Results

### Synfire Chain Simulation
- Demonstrates stable spike propagation across layers with biologically accurate noise and refractoriness.

### Neural Decoding
- Successfully decodes pointer velocity from recorded spike trains, showcasing the potential of spiking neural networks in neural decoding tasks.

---

## References

1. Diesmann et al. (1999): ["Stable propagation of synchronous spiking in cortical neural networks"](https://www.nature.com/articles/990101).
2. Glaser et al. (2020): ["Machine Learning for Neural Decoding"](https://doi.org/10.1523/ENEURO.0506-19.2020).

---
