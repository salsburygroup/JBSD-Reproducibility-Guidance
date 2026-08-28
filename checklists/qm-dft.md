# QM/DFT checklist

Use this checklist with the [universal computational checklist](universal-computational.md) for quantum-mechanical, density-functional, electronic-structure, or related calculations. For QM/MM work, also report the classical region and boundary treatment.

Do not submit the completed checklist.

## System and method

- [ ] **Required:** Provide the starting geometry and its provenance, atomic composition, charge, spin multiplicity, and electronic state as applicable.
- [ ] **Required:** Name the method, functional, basis set, pseudopotential or effective core potential, software, and version.
- [ ] **Conditional:** Report dispersion, solvation, relativistic, embedding, fragmentation, or finite-temperature treatments.
- [ ] **Conditional:** For periodic calculations, report the unit cell, boundary conditions, k-point sampling, plane-wave cutoff, smearing, and relevant convergence settings.
- [ ] **Required:** Report integration grids, self-consistent-field thresholds, occupation treatment, optimizer, geometry-convergence criteria, and other numerical settings that materially affect the result.
- [ ] **Conditional:** Describe QM/MM partitioning, link atoms, electrostatic embedding, boundary choices, and coupling between regions.
- [ ] **Conditional:** State how conformers, protonation states, spin states, or reaction pathways were generated and selected.
- [ ] **Conditional:** Verify stationary points with frequency calculations or another justified test when minima or transition states support the claims.

## Deposit

- [ ] **Required:** Provide input files, optimized or analyzed geometries, essential output files, and scripts used to extract or post-process results.
- [ ] **Required:** Map reported energies, structures, spectra, properties, and reaction coordinates to their source files.
- [ ] **Conditional:** Provide restart files, wavefunctions, densities, or checkpoints when they are needed to reproduce a principal result and repository limits permit.

## Evidence

- [ ] **Required:** Report numerical convergence and the precision used for reported differences.
- [ ] **Conditional:** Test basis-set, cutoff, grid, k-point, cell-size, functional, active-space, or embedding sensitivity when those choices could alter the conclusion.
- [ ] **Conditional:** Benchmark the method against higher-level calculations, reference datasets, or experiment when the claim depends on method accuracy.
- [ ] **Required:** Report uncertainty or method limitations at a level suited to the claimed precision.

