# Statistical Anti-Misuse

## Prohibited practices

1. Do not report P values without effect estimates and confidence intervals.
2. Do not report subgroup effects without interaction tests.
3. Do not claim causality from observational data without appropriate methods and caveats.
4. Do not ignore missing data or assume complete-case analysis is sufficient without justification.
5. Do not use parametric tests for clearly non-normal small samples without transformation or non-parametric alternatives.
6. Do not dichotomize continuous variables without clinical or methodological justification.
7. Do not perform multiple subgroup analyses without multiplicity correction.
8. Do not present Kaplan-Meier curves without reporting numbers at risk.
9. Do not report ROC AUC without 95% CI or calibration metrics.
10. Do not claim a prediction model is validated without independent validation data.

## Required practices

1. Always report the exact P value to three decimal places when P >= 0.001.
2. Always report effect estimates with 95% confidence intervals.
3. Always state the statistical software and version.
4. Always describe the handling of missing data.
5. Always justify the choice of statistical test.
6. Always report baseline characteristics with appropriate measures of spread.
7. Always describe the analysis population (intention-to-treat, per-protocol, etc.).

## Common errors to flag

- Post-hoc power analysis (do not calculate or report power after seeing the data)
- P-hacking or selective reporting
- Confounding without adjustment
- Overfitting in prediction models
- Violation of proportional hazards assumption without checking
- Inappropriate use of mean +/- SD for skewed data
