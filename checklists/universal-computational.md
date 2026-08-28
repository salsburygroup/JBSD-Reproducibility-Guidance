# Universal computational checklist

Use this checklist for every manuscript whose principal results depend on computation. Add the method-specific checklist or checklists that fit the work.

Do not submit the completed checklist.

## Manuscript

- [ ] **Required:** Include a Data Availability Statement. Name the archival repository and persistent identifier, or identify an editor-approved exception.
- [ ] **Required:** State the software, code, model, and parameter-set versions needed to understand or reproduce the principal results.
- [ ] **Required:** Describe the inputs, assumptions, preprocessing, calibration or training, analysis, and validation that materially affect the conclusions.
- [ ] **Conditional:** Report hardware architecture, operating system, compiler, numerical precision, or build details when they could materially affect the result.
- [ ] **Conditional:** Identify data, code, or records that cannot be shared and explain the restriction.

## Deposit

- [ ] **Required:** Archive the release supporting the paper in a repository that provides a persistent identifier and long-term preservation.
- [ ] **Required:** Include a README and file manifest. State the reuse terms or license where available.
- [ ] **Required:** Deposit the inputs, parameters, scripts, and data needed to reproduce the principal figures, tables, and reported results.
- [ ] **Required:** Map each principal manuscript result to its supporting files. The [manuscript-to-files map](../templates/manuscript-to-files-map.md) is one option.
- [ ] **Required:** Record software dependencies and run or analysis instructions.
- [ ] **Conditional:** Include random seeds, replicate identifiers, dataset splits, model checkpoints, or other state needed to reproduce a stochastic or trained workflow.
- [ ] **Conditional:** Document filtering, exclusions, transformations, alignment, subsampling, or other processing applied before analysis.
- [ ] **Recommended:** Include checksums for large or numerous files and a small test that confirms the environment and file paths.

## Evidence

- [ ] **Conditional:** Provide convergence, uncertainty, sensitivity, benchmarking, validation, or domain-of-applicability evidence only when it is customary for the method or needed to support a claim. Formal convergence tests and uncertainty estimates are not routine requirements for conventional molecular dynamics.
- [ ] **Required:** Distinguish technical reproduction from scientific validation. A runnable workflow or complete deposit does not by itself establish that the method or conclusion is valid.
