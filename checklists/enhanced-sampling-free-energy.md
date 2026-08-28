# Enhanced-sampling and free-energy checklist

Use this checklist with the [universal computational checklist](universal-computational.md) and, when applicable, the [molecular-dynamics checklist](molecular-dynamics.md).

Do not submit the completed checklist.

## Method

- [ ] **Required:** Identify the enhanced-sampling, rare-event, or free-energy method and the software version.
- [ ] **Required:** Define collective variables, states, restraints, bias potentials, schedules, alchemical pathways, lambda values, or exchange rules as applicable.
- [ ] **Required:** Report boundary choices, standard-state or finite-size corrections, estimators, integration procedures, and analysis conventions that affect the result.
- [ ] **Required:** Describe starting configurations, equilibration, sampling per window or replica, exchange attempts, initialization, and random seeds where applicable.
- [ ] **Conditional:** Explain how collective variables, pathways, or reference states were selected.

## Deposit

- [ ] **Required:** Provide inputs and parameters for every window, replica, walker, state, or alchemical leg.
- [ ] **Required:** Provide bias histories, work values, reduced potentials, weights, exchange records, or other primary analysis data required by the estimator.
- [ ] **Required:** Provide analysis scripts and the data behind the reported profiles, differences, rates, or state populations.
- [ ] **Required:** Map windows, replicas, and analysis outputs to the manuscript results.

## Evidence

- [ ] **Required:** For enhanced-sampling and free-energy results, report convergence evidence and uncertainty estimates suited to the method and reported quantity. This requirement does not extend to conventional molecular dynamics.
- [ ] **Conditional:** Show window or state overlap, exchange mixing, round trips, hysteresis, forward/reverse agreement, cycle closure, or comparable diagnostics when the method makes them relevant.
- [ ] **Conditional:** Test sensitivity to collective variables, starting states, analysis intervals, priors, or estimator choices when these choices could alter the conclusion.

