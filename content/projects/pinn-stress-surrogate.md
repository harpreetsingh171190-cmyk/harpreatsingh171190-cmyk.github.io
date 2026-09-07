---
title: "Physics-Informed Neural Network (PINN) for 2D Structural Stress"
date: 2026-09-07
draft: false
tags: ["PyTorch", "PINN", "Solid Mechanics", "FEA", "Deep Learning"]
description: "Surrogate modeling framework to predict 2D Von Mises stress fields and critical stress concentration factors around plate notches."
---

## Overview
Finite Element Analysis (FEA) simulations provide high-fidelity structural insights but are computationally expensive for iterative design exploration. This project develops a physics-informed surrogate capable of:
- **Accelerating Inference:** Spatial stress evaluations in <15 ms versus minutes in mesh solvers.
- **Physics Consistency:** Embedding Kirsch analytical decay formulations and Peterson finite-width corrections as inductive biases.
- **High Notch Fidelity:** Under 2% mean error in the critical stress concentration zone ($x/r \le 1.15$).

## Benchmark Performance
- **Global $R^2$ Score:** 0.9987
- **Root Mean Squared Error (RMSE):** 6.63 MPa
- **Mean Absolute Error (MAE):** 5.19 MPa

## Repository
View the full implementation, dataset, and Jupyter notebooks:
[GitHub Repository](https://github.com/harpreatsingh171190-cmyk/pinn-fea-stress-surrogate)
