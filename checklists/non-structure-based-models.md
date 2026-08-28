# Non-structure-based-model checklist

Use this checklist with the [universal computational checklist](universal-computational.md) for kinetic, statistical, network, systems, continuum, population, pharmacokinetic, or other models that are not primarily structure based.

Do not submit the completed checklist.

## Model and data

- [ ] **Required:** Define the model, state variables, equations, assumptions, constraints, and units.
- [ ] **Required:** Identify input data, provenance, versions, inclusion and exclusion rules, and preprocessing.
- [ ] **Required:** List fixed and fitted parameters, units, sources, bounds, priors, and initial values as applicable.
- [ ] **Required:** Describe calibration or fitting, objective or likelihood, solver or numerical method, stopping criteria, initial and boundary conditions, and software versions.
- [ ] **Conditional:** Describe discretization, mesh, time step, tolerances, or stochastic simulation settings when they affect the result.
- [ ] **Conditional:** Explain model selection, variable selection, regularization, or comparison among candidate models.

## Deposit

- [ ] **Required:** Provide executable code or a complete implementation description, configuration and input files, parameter tables, and analysis scripts.
- [ ] **Required:** Provide the data behind principal figures, tables, fitted values, forecasts, or simulations.
- [ ] **Required:** Map each reported result to the relevant model version, inputs, parameters, and output files.
- [ ] **Conditional:** Provide posterior samples, ensembles, covariance estimates, or fitted-state files when they are needed to reproduce uncertainty estimates.

## Evidence

- [ ] **Required:** Report goodness of fit, validation, uncertainty, and sensitivity analyses suited to the model and claims.
- [ ] **Conditional:** Assess identifiability, parameter correlation, overfitting, residual structure, or predictive calibration when relevant.
- [ ] **Conditional:** Validate against held-out data, an independent dataset, analytic limits, conservation laws, or established benchmarks as appropriate.
- [ ] **Required:** State the model's domain, limitations, and the consequences of assumptions that materially affect interpretation.

