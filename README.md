# Gradient Descent from Scratch 

This repository contains a step-by-step implementation of **Gradient Descent** for **Linear Regression**, built from scratch using **NumPy**, and compared against **scikit-learn’s LinearRegression**.

## Overview
Gradient Descent is an optimization algorithm used to minimize a **cost function** by iteratively adjusting model parameters. In the case of linear regression, we optimize the **slope (m)** and **intercept (b)** to minimize prediction errors.

This project:
- Implements Gradient Descent manually in Python.
- Uses **Mean Squared Error (MSE)** as the cost function.
- Compares the custom implementation against `sklearn.linear_model.LinearRegression`.
- Visualizes the fitted regression lines.

## Implementation Details
- Model Equation:  
  y = m * x + b

- Cost Function (MSE):  
  J(m, b) = (1 / 2n) * Σ (y - (mx + b))²

- Parameter Updates:  
  m := m - α * (∂J/∂m)  
  b := b - α * (∂J/∂b)  

  where α is the learning rate.

- Comparison: Results are benchmarked against scikit-learn’s built-in implementation.

## Results
- Custom Gradient Descent model converges to parameters close to the sklearn model.
- Both models produce nearly identical regression lines.
- Visualization shows:
  - Blue points = data samples  
  - Red line = custom gradient descent fit  
  - Green dashed line = sklearn fit  

## Requirements
- Python 3.x
- NumPy
- Matplotlib
- scikit-learn

Install dependencies with:
```bash
pip install numpy matplotlib scikit-learn
```

## Usage
Run the Jupyter Notebook:
```bash
jupyter notebook Gradient_Descend.ipynb
```



