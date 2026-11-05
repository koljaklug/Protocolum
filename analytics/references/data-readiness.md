# Data readiness

## Minimum inspection

Before choosing a method or chart, identify:

- source files, version/date, owner, and whether they are de-identified;
- one row's meaning (participant, visit, test, device run, task, or site);
- unique ID, timepoint/visit, treatment or test condition, and outcome fields;
- variable type, units, valid range, coding, and denominator for every endpoint;
- duplicate IDs, impossible values, outliers, missingness, withdrawals, exclusions, and protocol deviations;
- intended population: enrolled, treated/tested, analysed, per-protocol, or another declared set.

## Output: data-readiness ledger

| Item | Record | Status | Consequence |
|---|---|---|---|
| Unit of analysis | `[NEEDS INPUT]` | unresolved | analysis method cannot yet be chosen |
| Primary endpoint | `[NEEDS INPUT]` | unresolved | no primary inference or chart claim |
| Missing-data rule | `[NEEDS INPUT]` | unresolved | report descriptive missingness only |
| Version / provenance | `[NEEDS INPUT]` | unresolved | results are not reproducible |

Do not edit source data silently. Recommend a data-cleaning log with original value, reason, transformation, reviewer, and timestamp.
