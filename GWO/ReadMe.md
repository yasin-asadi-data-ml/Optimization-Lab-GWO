# 🐺 Grey Wolf Optimizer (GWO)

A clean Python implementation of the Grey Wolf Optimizer, a nature-inspired metaheuristic algorithm for optimization problems.

## Quick Start

```python
import numpy as np

# Define problem
dim = 5                # 5 variables to optimize
n_wolves = 10          # 10 wolves in the pack
max_iter = 30          # 30 iterations
bounds = (-10, 10)     # Search space boundaries

# Run optimization
best_solution, best_fitness = GWO(
    objective_function, 
    dim, 
    n_wolves, 
    max_iter, 
    bounds[0], 
    bounds[1]
)
```

## Features
- 🎯 Minimize any function by replacing `objective_function()`
- 🐺 Simulates wolf pack hierarchy (α, β, δ leaders)
- ⚡ Efficient NumPy vectorized operations
- 📏 Automatic boundary constraints
- 🔧 Easy parameter tuning

## Customize Your Problem

```python
def your_function(x):
    """Your custom objective to minimize"""
    return np.sum(x**2)  # Replace with your function

# Run with your function
solution = GWO(your_function, dim=10, ...)
```

## Parameters
- `dim`: Problem dimensions (1-1000+)
- `search_agents_no`: Number of wolves (10-50)
- `max_iter`: Iterations (50-1000)
- `lower/upper_bound`: Search space limits

## Applications
- Function optimization
- Machine learning hyperparameter tuning
- Engineering design
- Feature selection

## Installation
```bash
pip install numpy
```

*Copy the full GWO code into your project and start optimizing!*