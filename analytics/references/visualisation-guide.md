# Visualisation guide

Choose a chart that preserves the unit of observation, denominator, uncertainty, and distribution. Prefer direct labels and clear titles that state outcome, population, timepoint, and scale.

| Question | Recommended visual | Include |
|---|---|---|
| How participants/tests moved through the study | flow diagram | screened/enrolled/tested/analysed and reasons for loss/exclusion |
| What the distribution looks like | jittered points + summary, histogram, or density | individual observations where privacy permits; n and units |
| How values changed within individuals | spaghetti plot with summary trajectory | participant links, timepoints, missing observations |
| How groups compare at one timepoint | point/range estimate plot | effect estimate, confidence interval, denominator, reference line |
| Whether a prototype passed defined criteria | run chart or dot plot with acceptance band | test condition, threshold source, pass/fail and failed runs |
| Task success and use errors | stacked bars plus error table | users/tasks, denominator, severity, mitigation status |
| Agreement between two measures | difference-versus-mean plot | bias, limits/uncertainty, units; not correlation alone |
| Diagnostic performance | sensitivity/specificity forest or ROC with uncertainty | reference standard, threshold, confidence intervals, sample flow |

## Design rules

- Use a zero baseline for bars; avoid bars for continuous distributions when raw points fit.
- Avoid 3D effects, dual y-axes, truncated scales that exaggerate differences, and color alone to encode groups.
- Use colour-blind-safe contrast plus shapes or direct labels. Include a legend only when direct labels are impractical.
- Make uncertainty visible. State whether error bars are SD, SE, CI, range, or another interval.
- Declare transformations (e.g., log scale) and display units. Never obscure missing data or failures.

## Figure specification template

`Figure [number]. [Question answered]. Population/tests: [denominator]. Outcome: [definition, unit, timepoint]. Mark: [point/line/bar]. Encodings: [group, colour, shape]. Summary/uncertainty: [method]. Reference/acceptance line: [source]. Missing/excluded: [rule]. Caption claim boundary: [what this figure does and does not show].`
