# Coarse-grained-model checklist

Use this checklist with the [universal computational checklist](universal-computational.md). Add the [molecular-dynamics checklist](molecular-dynamics.md) when the coarse-grained work uses molecular dynamics.

Do not submit the completed checklist.

## Model

- [ ] **Required:** Define the coarse-graining level, mapping from the underlying system, bead types or state variables, and governing interactions.
- [ ] **Required:** Identify the model, force field, parameter-set version, software, and any modifications.
- [ ] **Required:** Describe how parameters were derived, fitted, transferred, or selected. Cite or deposit the reference data used in parameterization.
- [ ] **Required:** State the thermodynamic state, composition, boundary conditions, restraints, and initialization.
- [ ] **Conditional:** Describe backmapping or reconstruction when atomistic structures or observables are part of the claims.
- [ ] **Conditional:** Explain the interpretation of model time or kinetic observables when the coarse-grained dynamics do not map directly to physical time.

## Sampling and deposit

- [ ] **Required:** Report replica count, sampling length, initialization, and random seeds where applicable.
- [ ] **Required:** For coarse-grained molecular dynamics, pool compatible independent replicas for the primary analysis unless the scientific question or a diagnostic result requires separate treatment.
- [ ] **Required:** Deposit mappings, topology and parameter files, starting states, run inputs, analysis scripts, and data supporting the principal results.
- [ ] **Required:** Document conversions between coarse-grained and higher-resolution representations.

## Evidence

- [ ] **Required:** State the model's intended domain and limitations.
- [ ] **Required:** Validate the model against atomistic calculations, experimental data, held-out conditions, or another justified reference suited to the claims.
- [ ] **Conditional:** Report convergence tests, uncertainty estimates, or between-replica variation only when the method, observable, or claim makes them scientifically appropriate. They are not routine requirements for coarse-grained molecular dynamics.
- [ ] **Conditional:** Test sensitivity to mapping, resolution, parameter set, or state conditions when those choices could alter the conclusion.
