# Stochastic Epidemic Modeling with the SIRD Model

A computational study of epidemic dynamics using the **Susceptible–Infected–Recovered–Deceased (SIRD)** compartmental model, combining deterministic ordinary differential equations with stochastic simulation via the **Gillespie stochastic simulation algorithm (SSA)**.

**Authors:** Martina Balsamello and Matteo Zabban. This is a collaborative academic project.

## Overview

Deterministic compartmental models describe average epidemic trajectories, while stochastic models capture variability across outbreaks, particularly when infections are rare. This project explores both perspectives and examines epidemic trajectories and the probability of early extinction under different model parameters.

## Methods

- Deterministic SIRD dynamics solved numerically with `scipy.integrate.solve_ivp`.
- Stochastic SIRD trajectories generated using Gillespie's direct method.
- Repeated stochastic simulations to examine variability and early extinction.
- Parameter sensitivity analysis and visualizations of epidemic dynamics.
- Interactive parameter exploration using Jupyter widgets in the main notebook.

## Repository structure

```text
stochastic-epidemic-modeling/
├── README.md
├── requirements.txt
├── .gitignore
└── notebooks/
    ├── Balsamello_Zabban.ipynb  # Main project notebook
    ├── STOCH.ipynb               # Related SIRD exploration
    └── SIRD.ipynb                # Additional simulation experiments
```

## Getting started

Install dependencies:

```bash
pip install -r requirements.txt
```

Open `notebooks/Balsamello_Zabban.ipynb` in Jupyter Notebook or JupyterLab. The other notebooks document related experiments and development work. Run cells in order; interactive plots require a Jupyter environment with widget support.

## Model assumptions and limitations

The model assumes a closed, well-mixed population and simplified infection, recovery, and death processes. Results are **illustrative simulations**, not calibrated epidemiological forecasts or clinical guidance.

## Notes

Notebook code is preserved from the original project; student identification numbers have been removed from markdown headings for public sharing. Numerical results depend on the selected parameters and simulation randomness.
