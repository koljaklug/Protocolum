# Quality Gates

## Gate 1: Safety and compliance

Before any task, run the preflight checklist from safety-and-compliance.md.

If any item fails, stop and ask the user to resolve before proceeding.

## Gate 2: Minimum inputs

Before producing substantive content, verify minimum required inputs from minimum-inputs.md.

If essential inputs are missing, ask up to 3 targeted questions or proceed only with explicit user consent for a rough draft.

## Gate 3: Statistical integrity

Before presenting any statistical result, verify:

1. The statistical test matches the data type and design.
   - Continuous + 2 groups: t-test or Mann-Whitney U
   - Continuous + 3+ groups: ANOVA or Kruskal-Wallis
   - Categorical: chi-square or Fisher exact
   - Paired/repeated: paired t-test, Wilcoxon, mixed models
   - Survival: Kaplan-Meier, log-rank, Cox
   - Correlation: Pearson, Spearman

2. If P < 0.05 is reported, the effect estimate and 95% CI are also reported.

3. If subgroup analyses are reported, an interaction test is mentioned.

4. If multiple comparisons are made, a correction method is stated.

5. If missing data are present, the handling method is stated.

If any of these are violated, flag the issue and suggest the correct approach.

## Gate 4: Reporting guideline alignment

Before finalizing any section, check alignment with the relevant reporting guideline:

- RCT: CONSORT
- Observational: STROBE
- Systematic review/meta-analysis: PRISMA
- Case report: CARE
- Diagnostic accuracy: STARD
- Prediction model: TRIPOD

If the user specifies a target journal, also check the journal's specific requirements from journal-requirements.md.

## Gate 5: Translation and bilingual accuracy

Before delivering a translated or polished manuscript:

1. Verify that medical terms use the correct target-language equivalents.
   - English: MeSH preferred terms
   - Chinese: National Medical Terminology Committee standards

2. Verify that abbreviations are expanded on first use in the target language.

3. Verify that statistical notation follows the target journal's convention.
   - English: P italic, 95% CI, mean +/- SD
   - Chinese: P italic, 95% CI, mean +/- SD or median (IQR)

4. Verify that numbers and units follow the target format.
   - English: space between number and unit (5 mL)
   - Chinese: number + unit without space (5mL) or with narrow space

5. Verify that references and citations are not fabricated.

## Gate 6: Output completeness

Before finishing a task, verify:

1. The output contains all sections requested by the user.
2. No section is left as a placeholder like `[TBD]` unless explicitly marked as needing user input.
3. If the user provided data, all numbers in the output match the input.
4. If the task is a review or checklist, all items are addressed with a clear status.
