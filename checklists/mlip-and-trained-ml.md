# MLIP and trained-ML checklist

Use this checklist with the [universal computational checklist](universal-computational.md) for machine-learned interatomic potentials and other trained AI or machine-learning models.

Do not submit the completed checklist.

## Task, data, and model

- [ ] **Required:** Define the prediction task, outputs, intended domain, and role of the trained model in the manuscript's claims.
- [ ] **Required:** Identify every training, validation, test, and external dataset; give its source, version, license or access terms, and selection criteria.
- [ ] **Required:** Describe label generation, preprocessing, normalization, filtering, deduplication, augmentation, and excluded records.
- [ ] **Required:** Provide the dataset split rules and identifiers. Explain how related structures, trajectories, patients, experiments, or other grouped observations were kept from leaking across splits.
- [ ] **Required:** Describe the architecture, descriptors or features, loss function, optimizer, schedule, stopping rule, hyperparameters, software, and dependency versions.
- [ ] **Required:** Report initialization and random seeds where available.
- [ ] **Conditional:** For machine-learned potentials, define the reference electronic-structure method, sampled chemical and configurational space, active-learning or selection procedure, and units.

## Deposit

- [ ] **Required:** Provide training and evaluation code, configuration files, split definitions, preprocessing scripts, and inference scripts.
- [ ] **Conditional:** Provide training data or stable identifiers for each source dataset where licensing, privacy, and size permit.
- [ ] **Conditional:** Provide trained weights or checkpoints where legally and technically permitted. If they cannot be shared, explain the constraint and what can be reproduced without them.
- [ ] **Required:** Provide predictions and reference values behind the principal metrics, plots, tables, and downstream analyses.
- [ ] **Recommended:** Include a small inference example with expected output.

## Evidence

- [ ] **Required:** Report performance separately for training, validation, test, and external data as applicable. Define every metric.
- [ ] **Required:** Compare against relevant baselines or established methods when the manuscript claims improved performance.
- [ ] **Required:** State the domain of applicability and evaluate failures, extrapolation, or out-of-distribution behavior relevant to the intended use.
- [ ] **Conditional:** Report calibration or predictive uncertainty when confidence estimates affect interpretation or use.
- [ ] **Conditional:** Repeat training or evaluation with independent seeds when stochastic variation could change the conclusion.
- [ ] **Conditional:** For machine-learned potentials, test stability and relevant physical observables in simulations beyond pointwise test errors.

