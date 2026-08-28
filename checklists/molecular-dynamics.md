# Molecular-dynamics checklist

Use this checklist with the [universal computational checklist](universal-computational.md) for conventional atomistic or closely related molecular-dynamics studies.

Do not submit the completed checklist.

## System and methods

- [ ] **Required:** Identify the starting structure or model and its provenance.
- [ ] **Required:** Describe missing-region modeling, protonation, ligands or cofactors, solvent or membrane, ions, salt concentration, and full system composition as applicable.
- [ ] **Required:** Name the force field and parameter-set version. Provide and validate nonstandard parameters.
- [ ] **Required:** Report minimization, equilibration, and production procedures; ensemble; integrator; time step; constraints; thermostat and barostat algorithms and coupling parameters; cutoffs; and long-range electrostatics.
- [ ] **Required:** Name the simulation engine and version.
- [ ] **Required:** Report the number and length of independent replicas and how each was initialized.
- [ ] **Required:** Use at least three independent replicas for conventional molecular dynamics, or give a scientific rationale for another replication or sampling strategy.
- [ ] **Conditional:** Report random seeds, or how they were seeded, when they are available or needed to distinguish replicas.
- [ ] **Required:** Pool compatible independent replicas for the primary analysis unless the scientific question or a diagnostic result requires separate treatment. Describe the pooling, weighting, equilibration removal, and other frame exclusions.
- [ ] **Required:** Explain why the model, force field, sampling strategy, and algorithms fit the scientific question.

## Deposit

- [ ] **Required:** Provide compatible starting structures, topologies, force-field files, nonstandard parameters, and system-preparation records.
- [ ] **Required:** Provide production inputs, essential settings, restraints, applied biases, dependency information, seeds where applicable, and replicate mappings.
- [ ] **Required:** Provide the scripts and data underlying the principal results and map them to manuscript figures and tables.
- [ ] **Conditional:** Deposit complete production trajectories with compatible topology and structure files where repository capacity allows.
- [ ] **Conditional:** If complete trajectories cannot be deposited, explain why and provide the claim-supporting analysis data plus a trajectory subset. Representative structures or movies alone are insufficient.
- [ ] **Required:** Document removed components, filtered frames, alignment, reimaging, clustering, and subsampling.

## Evidence

- [ ] **Conditional:** Add convergence tests or uncertainty estimates only when the method, observable, or claim makes them scientifically appropriate. They are not routine requirements for conventional molecular dynamics.
- [ ] **Conditional:** Show between-replica variation only when it is needed to diagnose a sampling problem, justify separate treatment or exclusion of a run, or support a claim about heterogeneity.
- [ ] **Conditional:** Compare simulation conclusions with relevant experimental evidence when it is available.
