---
name: protocolum-analytics-direct
description: Plan and review statistical analyses and data visualisations for small clinical studies, conference research, and medical-device prototype evaluations. Use for data-readiness checks, analysis plans, results tables, figure specifications, and interpretation review; do not use to fabricate data or make clinical or regulatory claims.
---

# Protocolum Analytics

## Purpose

Turn a supplied dataset, data dictionary, results table, or study summary into an auditable analysis and visualisation plan. This skill supports reproducible thinking and clear communication; it does not replace a biostatistician for consequential or complex inference.

## Workflow

1. Run the data-integrity checks in `references/data-readiness.md`.
2. Identify the study and evidence type: pilot clinical study, observational study, bench verification, simulated use, usability, feasibility, or clinical performance.
3. Read the matching mode in `references/analysis-playbook.md`. For chart requests, also read `references/visualisation-guide.md`.
4. Create an analysis ledger before interpreting results: question, analysis unit, population/tests, endpoint definition, timepoint, denominator, comparison, method, missing-data handling, and limitations.
5. Produce only results supported by supplied data. If data are unavailable, provide executable analysis specifications or table/figure shells—not invented values.
6. Apply `references/review-checklist.md` and name any necessary expert review.

## Routes

| Request | Read |
|---|---|
| Inspect data quality, variables, or missingness | `data-readiness.md` |
| Plan clinical/pilot or observational analysis | `analysis-playbook.md` — Clinical studies |
| Analyse bench, reliability, diagnostic, usability, or prototype evaluation data | `analysis-playbook.md` — Prototype evidence |
| Design a figure, dashboard, poster chart, or results table | `visualisation-guide.md` |
| Check a completed analysis or result interpretation | `review-checklist.md` |

## Non-negotiables

- Do not impute, drop, transform, or combine records without stating the rule and its consequence.
- Keep the participant, device, site, task, and observation units distinct. Clustered or repeated data require an appropriate method or explicit expert review.
- Pair estimates with denominators and uncertainty where inference is claimed. Report failures, harms, use errors, exclusions, and missing data.
- Treat pilot and feasibility analyses as estimates of feasibility/precision unless the design and evidence support stronger conclusions.
- Keep exploratory analyses visibly exploratory. Never search for a favorable result, then present it as pre-specified.
- Do not infer safety, effectiveness, generalisability, clearance, or approval from a chart alone.
