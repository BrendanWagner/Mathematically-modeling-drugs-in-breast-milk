# Modeling Trikafta Transfer from Maternal Plasma to Breast Milk

This project simulates the pharmacokinetics of **Trikafta** (a cystic fibrosis therapy) in a **breastfeeding context**. Using a simple ODE-based model, it estimates how the concentration of the drug in a mother’s blood translates into the concentration present in breast milk over time.

The notebook demonstrates the process of:
- Defining a pharmacokinetic model with limited data,  
- Implementing it in Python with `NumPy` and `SciPy`,  
- Solving the ODE numerically, and  
- Visualizing the resulting profiles with `Matplotlib`.

---

## Project Overview

The model assumes daily maternal dosing and exponential decay of plasma concentration.  
A small fraction of the drug is assumed to pass into breast milk, where it also decays over time.

Key steps:
1. **Model maternal concentration** — exponential decay plus repeated dosing.  
2. **Set up a one-compartment ODE** for drug transfer to milk.  
3. **Numerically solve** the ODE using `solve_ivp`.  
4. **Visualize** the results to compare plasma vs. milk concentration curves.

All parameter values are approximate and chosen for illustrative modeling purposes rather than pharmacological accuracy.

---

## Methods

- **Language:** Python  
- **Libraries:**  
  - `NumPy` for vectorized math  
  - `SciPy` for numerical ODE solving  
  - `Matplotlib` for plotting results  

The notebook focuses on **conceptual modeling**—not on reproducing clinical data—making it a useful example of how mathematical modeling and computational tools can be used to explore pharmacokinetic systems.
