# Option Pricing with Finite Difference Methods

This notebook was part of my Computational Finance course in my 
M.Sc. Quantitative Finance program. It covers numerical methods 
for option pricing, with a focus on solving PDEs using finite 
difference schemes.

## What this covers

- **Monte Carlo methods** for computing option sensitivities (delta) 
  using finite difference, infinitesimal perturbation, and likelihood 
  ratio estimators
- **Explicit finite difference scheme** for pricing European options 
  — including stability analysis
- **Crank-Nicolson scheme** — more stable than explicit FD, requires 
  solving a tridiagonal linear system at each time step
- **Longstaff-Schwartz algorithm** for American option pricing via 
  Monte Carlo simulation
- **Richardson extrapolation** to improve convergence of binomial 
  tree pricing

## What I found interesting

The Crank-Nicolson scheme required implementing a tridiagonal matrix 
solver from scratch (Thomas algorithm), which turned out to be very 
similar in structure to what finite element solvers do in engineering 
applications — assembling and solving sparse linear systems efficiently.

## Dependencies

```bash
pip install numpy scipy matplotlib
```

## How to run

Open the notebook in Jupyter:

```bash
jupyter notebook pde_option_pricing_solver.ipynb
```

## Course context

This was Week 10 of the Computational Finance module, covering 
Chapters 5 and 6 of the lecture notes - numerical methods for 
PDEs and sensitivity analysis.

**Program**: M.Sc. Quantitative Finance  
**University**: Kiel University
