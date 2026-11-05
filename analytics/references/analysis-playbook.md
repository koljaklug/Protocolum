# Analysis playbook

## Clinical and pilot studies

Start with the decision question, then define the primary outcome, timepoint, analysis population, and estimand. For each outcome, specify the metric and method before seeing results.

| Outcome / design | Useful summaries | Typical analysis consideration |
|---|---|---|
| Continuous outcome, one timepoint | n, mean (SD) or median (IQR), distribution plot | adjusted or unadjusted difference with confidence interval; verify assumptions |
| Binary outcome | events/total, risk or proportion | report risk difference/ratio or odds ratio with confidence interval |
| Repeated measures | participant trajectories and time-specific summaries | account for within-participant correlation; do not treat visits as independent |
| Time-to-event | events, median follow-up, numbers at risk | define origin, censoring, and event; use appropriate survival methods |
| Feasibility outcome | recruitment, retention, adherence, completion | compare to pre-declared progression criteria; present precision rather than efficacy claims |

Report the analysis population, each denominator, missing data, deviations, safety events, and whether any analysis was exploratory. Obtain a biostatistician review for small samples with adjustment, clustering, multiplicity, causal claims, time-to-event inference, or substantive missing data.

## Prototype evidence

Match analysis to the evidence level and unit.

| Evidence | Core outputs | Common mistake to avoid |
|---|---|---|
| Bench verification | test conditions, runs, acceptance criteria, pass/fail, measurement uncertainty | claiming clinical performance from bench data |
| Reliability / agreement | paired observations, repeatability, reproducibility, uncertainty | reporting correlation as agreement |
| Usability / simulated use | users, tasks, success, use errors, close calls, mitigations | reporting average success without the error narrative |
| Feasibility | workflow completion, recruitment, timing, implementation barriers | framing preliminary signals as effectiveness |
| Diagnostic / clinical performance | reference standard, participant flow, sensitivity/specificity and uncertainty | omitting indeterminate results or selection flow |

For every failed run, use error, deviation, adverse event, or indeterminate result, report the denominator and disposition. Do not remove inconvenient records without a documented pre-specified rule.

## Analysis-plan shell

1. Question and claim boundary
2. Dataset version and provenance
3. Analysis unit and population(s)
4. Endpoint definitions and timepoints
5. Primary summaries/effect measures and uncertainty
6. Model/test and assumptions to check
7. Missing data, exclusions, and deviations
8. Safety/failure/use-error summaries
9. Sensitivity and exploratory analyses
10. Tables, figures, and interpretation limits
