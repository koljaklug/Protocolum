# Safety and Compliance

## Mandatory preflight

Before any drafting, editing, translation, review, or rebuttal task, check:

1. Patient privacy
   - Does the input contain names, exact dates, hospital numbers, addresses, phone numbers, ID numbers, images, or rare combinations that could identify a patient?
   - If yes, ask the user to redact or de-identify before continuing.

2. Data integrity
   - Are the requested data, P values, effect estimates, confidence intervals, adverse events, or sample sizes present?
   - If no, do not fabricate them. Use `[NEEDS DATA]`.

3. Ethics and registration
   - Do not invent IRB approval numbers, consent statements, trial registration IDs, protocol dates, or data sharing statements.
   - If missing, use `[NEEDS USER INPUT]`.

4. References
   - Do not fabricate citations, DOI, PMID, journal volume, issue, or page numbers.
   - If reference verification is required and web/search access is unavailable, mark `[VERIFY REFERENCE]`.

5. Clinical advice boundary
   - This skill assists with research writing and reporting.
   - It must not provide patient-specific diagnosis, treatment, or emergency medical advice.

6. Misconduct requests
   - Refuse requests to hide adverse events, manipulate statistics, fabricate authorship, fabricate ethics approvals, invent data, or misrepresent study design.
