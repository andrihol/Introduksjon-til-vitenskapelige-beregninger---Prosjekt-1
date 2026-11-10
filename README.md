
# Physics-Informed Neural Networks (PINNs)

**TMA4320 – Introduction to Scientific Computation | NTNU**

## Overview

Academic group project exploring the use of numerical methods, neural networks, and Physics-Informed Neural Networks (PINNs) to model heat distribution in a two-dimensional room.

The project investigates how physical laws can be incorporated into machine learning models to improve temperature predictions based on limited and noisy sensor data.

Three modelling approaches were studied:
1. Finite Difference Method (FDM)
2. Neural Networks (NN)
3. Physics-Informed Neural Networks (PINN)

## Technologies

- Python
- JAX
- NumPy
- Matplotlib
- Neural Networks
- Numerical Methods
- Scientific Computing

## Project Components

### 1. Numerical Heat Equation Solver

Worked with a finite difference solver to simulate heat distribution over time.

The work included:
- Discretizing the two-dimensional heat equation
- Applying implicit Euler time integration
- Incorporating Robin boundary conditions
- Solving linear systems for temperature evolution
- Generating synthetic temperature sensor data
- Visualizing heat distribution over time

### 2. Neural Networks

Implemented and trained a neural network to predict temperature distributions from simulated sensor measurements.

The work included:
- Building a fully connected neural network using JAX
- Defining loss functions for sensor data and initial conditions
- Training the network to approximate temperature fields
- Investigating the effects of sensor placement and measurement noise
- Comparing neural network predictions with numerical simulations

### 3. Physics-Informed Neural Networks

Extended the neural network approach by incorporating physical constraints based on the heat equation.

The work included:
- Integrating physical laws into the training objective
- Evaluating differential equation residuals
- Combining data-driven and physics-based loss functions
- Investigating the influence of training parameters
- Comparing PINN predictions with conventional neural networks and numerical solutions

## Key Findings

- Numerical simulations provided a reference solution for evaluating machine learning models.
- Neural networks trained on limited sensor data struggled to reproduce realistic temperature distributions.
- Increasing the number of sensors improved the quality of temperature predictions.
- Measurement noise influenced training losses and prediction accuracy.
- Physics-informed modelling demonstrated the importance of incorporating physical constraints when learning from limited observations.

## Project Structure

The project is organized into the following components:

- `src/project/` – Core implementations of the numerical solver, neural networks, and loss functions
- `scripts/` – Scripts for running simulations, training models, and visualizing results
- `tests/` – Automated tests
- `config.yaml` – Physical parameters and model configurations
- `pyproject.toml` – Python dependencies and project configuration
- `Project_Report.pdf` – Mathematical derivations, experiments, results, and discussion

## Academic Context

Completed as a group project in TMA4320 – Introduction to Scientific Computation at the Norwegian University of Science and Technology (NTNU).

The project combines numerical mathematics, differential equations, machine learning, and scientific programming to investigate data-driven and physics-informed approaches to heat transfer modelling.

**Group members:** Andrine Holen, Selma Holmen Berg, and Emily Ann Mercer.
