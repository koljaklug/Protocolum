# Prompt Library

## Module 1: Study Design & Protocol

### Prompt 1: Clinical Study Design Consultation

**Role**: You are a clinical research methodology expert with 20 years of experience, proficient in all types of clinical study designs and their applicable scenarios.

**Task**: Based on the research idea I provide, recommend the most appropriate study design type and give a detailed study protocol framework.

**Input**:

- Research question: \[describe your clinical question]
- Study population: \[target patient population]
- Available resources: \[data/sample/time/funding]
- Target journal tier: \[top-tier/specialty/Chinese core]

**Output format**:

**Recommended study design**

- Design type: \[RCT/cohort/case-control/cross-sectional/case series/etc.]
- Rationale: \[why this design best fits your research question]
- Evidence level: \[evidence level in evidence-based medicine]

**Study protocol framework**

1. Study objectives and hypotheses
   - Primary objective
   - Secondary objectives
   - Hypotheses (H0 and H1)
2. Study design details
   - Design type and schematic
   - Inclusion/exclusion criteria (specific, quantifiable)
   - Sample size calculation basis and formula
   - Randomization and blinding plan (if applicable)
3. Interventions/exposures and outcomes
   - Intervention or exposure definition
   - Primary outcome (Primary Endpoint)
   - Secondary outcomes
   - Follow-up plan and time points
4. Statistical plan
   - Statistical software
   - Analysis methods (descriptive and inferential statistics)
   - Missing data handling
   - Subgroup analysis plan
   - Interim analysis plan (if applicable)
5. Ethics and registration
   - Ethics approval points
   - Clinical trial registration platform recommendation
   - Informed consent process
6. Quality control
   - Data management plan
   - Bias control measures
   - Safety monitoring (if applicable)

**Precautions**

- \[List 3-5 common pitfalls for this design and how to avoid them]

***

### Prompt 2: Sample Size Calculation

**Role**: You are a biostatistics expert specializing in medical research sample size calculation and statistical power analysis.

**Task**: Based on the research parameters I provide, calculate the required sample size and provide statistical justification.

**Input**:

- Study design type: \[RCT/cohort/case-control/cross-sectional/diagnostic test/etc.]
- Primary outcome: \[continuous/binary/survival/repeated measures/etc.]
- Expected effect size: \[specific value or clinically meaningful minimum difference]
- Significance level (alpha): \[usually 0.05]
- Statistical power (1-beta): \[usually 0.80 or 0.90]
- Other parameters: \[e.g., dropout rate, group ratio, baseline rate, etc.]

**Output format**:

**Sample size calculation results**

- Sample size per group: N = ?
- Total sample size: N\_total = ?
- Adjusted for dropout rate (e.g., 20%): N\_adjusted = ?

**Calculation basis**

- Statistical formula/software used
- Parameter setting rationale
- Effect size source (literature basis or clinical consensus)

**Sensitivity analysis**

- Sample size when effect size changes +/- 20%
- Sample size when power changes (0.80 vs 0.90)

**Recommendations**

- Is it feasible?
- Alternative suggestions if sample size is too large

***

## Module 2: Structured Paper Writing

### Prompt 3: Structured Abstract

**Role**: You are a senior medical journal editor, skilled at writing structured abstracts that meet international medical top-tier journal standards.

**Task**: Based on the research information I provide, write a structured abstract in both Chinese and English.

**Input**:

- Study type: \[RCT/cohort/case-control/cross-sectional/basic experiment/case report/systematic review]
- Study objective: \[1-2 sentences]
- Methods: \[design, subjects, intervention/exposure, outcome measures, statistical methods]
- Main results: \[key data, with statistical values and P values]
- Core conclusion: \[answer the research question, avoid over-interpretation]
- Target journal: \[NEJM/Lancet/JAMA/BMJ/Stroke/Neurology/中华医学杂志/etc.]

**Constraints**:

1. English abstract 250-350 words (top-tier) or 400-500 words (Chinese journal English)
2. Chinese abstract 400-500 characters (CMA series)
3. Default structure: Background/Objective, Methods, Results, Conclusion
4. JAMA override: if the target journal is JAMA, use Importance, Objective, Design Setting and Participants, Interventions, Main Outcomes and Measures, Results, Conclusions and Relevance
5. Must include specific data (e.g., OR=1.32, 95% CI: 1.05-1.67, P=0.015)
6. No abbreviations (full name on first use)
7. No references cited
8. Third person, no "this paper" or "we"

**Output format**:

**Structured Abstract (English)**
\[Use the heading structure matching the target journal. Default:]
**Background/Objective**: \[content]
**Methods**: \[content]
**Results**: \[content]
**Conclusion**: \[content]

\[JAMA override, if applicable:]
**Importance**: \[content]
**Objective**: \[content]
**Design, Setting, and Participants**: \[content]
**Interventions**: \[content]
**Main Outcomes and Measures**: \[content]
**Results**: \[content]
**Conclusions and Relevance**: \[content]

**结构化摘要 (中文)**
**目的**: \[content]
**方法**: \[content]
**结果**: \[content]
**结论**: \[content]

**Abstract quality check**

- [ ] Does the heading structure match the target journal?
- [ ] Contains specific data?
- [ ] Answers the research question?
- [ ] Conclusion based on results, no over-interpretation?
- [ ] Word count meets target journal requirements?

***

### Prompt 4: Introduction

**Role**: You are a clinical medical writing expert, skilled at writing logically rigorous medical paper introductions.

**Task**: Based on the research background I provide, write an introduction that conforms to the IMRaD structure.

**Input**:

- Research disease/topic: \[specific disease or medical problem]
- Disease burden: \[epidemiological data]
- Current treatment/diagnostic status: \[current clinical practice]
- Existing research limitations: \[literature review points]
- Innovation of this study: \[difference from existing research]
- Study objective: \[specific, quantifiable goal]

**Constraints**:

1. Logical chain: Background -> Problem -> Gap -> Study Purpose
2. "Funnel" structure: from macro to micro
3. Cite core literature from the past 5 years (mark \[CITATION NEEDED])
4. Last paragraph clearly states study objectives and hypotheses
5. Avoid presenting result data in the introduction
6. Chinese journals: introduction usually <=500 characters; English top-tier: usually 3-4 paragraphs, \~500-800 words

**Output format**:

**Introduction (English)**
\[Written in funnel structure]

**引言 (中文)**
\[Corresponding Chinese version]

**Introduction structure check**

- [ ] Paragraph 1: Clinical importance and epidemiology of the disease/problem
- [ ] Paragraph 2: Current research progress and knowledge status
- [ ] Paragraph 3: Deficiencies/gaps in existing research (Gap)
- [ ] Paragraph 4: Study objectives and hypotheses

***

### Prompt 5: Methods

**Role**: You are a medical research methodology writing expert, familiar with CONSORT/STROBE/PRISMA and other reporting guidelines.

**Task**: Based on the research information I provide, write a detailed Methods section.

**Input**:

- Study design: \[specific design type]
- Study subjects: \[inclusion/exclusion criteria]
- Intervention/exposure: \[detailed description]
- Control: \[control group setup]
- Outcome measures: \[primary/secondary outcomes and measurement methods]
- Statistical methods: \[analysis plan]
- Ethics information: \[IRB approval number]
- Registration information: \[clinical trial registration number]

**Constraints**:

1. Must include ethics approval statement and informed consent description
2. Must include clinical trial registration number (if applicable)
3. Statistical methods must specify software version, test name, significance level
4. Use past tense
5. Detailed enough for others to replicate
6. Follow target journal's methodological reporting guidelines (CONSORT/STROBE, etc.)

**Output format**:

**Methods**

**Study Design and Participants**
\[Study design, setting, inclusion/exclusion criteria]

**Ethics and Registration**
\[Ethics approval, informed consent, trial registration]

**Interventions/Exposures**
\[Detailed description of intervention or exposure]

**Outcomes**
\[Definition and measurement of primary and secondary outcomes]

**Sample Size**
\[Sample size calculation basis]

**Statistical Analysis**
\[Statistical software, analysis methods, missing data handling, subgroup analysis]

**Methodology checklist**

- [ ] Meets CONSORT/STROBE/PRISMA requirements?
- [ ] Are inclusion/exclusion criteria specific and quantifiable?
- [ ] Are outcome measures clear and measurable?
- [ ] Do statistical methods match data types?

***

### Prompt 6: Results

**Role**: You are a medical statistical writing expert, skilled at objectively and accurately presenting clinical research results.

**Task**: Based on the data I provide, write a Results section that meets medical journal standards.

**Input**:

- Baseline characteristics: \[demographic/clinical characteristics]
- Primary outcome results: \[key data]
- Secondary outcome results: \[supporting data]
- Subgroup analysis results: \[if applicable]
- Safety data: \[adverse events, etc.]
- Statistical results: \[P values, OR/HR, 95% CI, etc.]

**Constraints**:

1. Objective presentation, no interpretation or discussion (save for Discussion)
2. Logical order: baseline characteristics -> primary outcome -> secondary outcomes -> subgroup/safety
3. Report appropriate statistical quantities. Prefer effect estimates with 95% confidence intervals; report P values only when hypothesis testing is prespecified and applicable
4. Text and figures/tables complement each other, no duplication
5. Use past tense
6. Chinese journals: P values generally expressed as P>0.05, P<0.05, P<0.01

**Output format**:

**Results**

**Baseline Characteristics**
\[Demographic and clinical baseline characteristics table description]

**Primary Outcome**
\[Primary outcome results, with effect size and confidence interval]

**Secondary Outcomes**
\[Secondary outcome results]

**Subgroup Analyses**
\[Subgroup analysis results]

**Safety**
\[Safety data]

**Results presentation check**

- [ ] Is it objective without interpretation?
- [ ] Does it include precise statistical values?
- [ ] Is data consistent with figures/tables?
- [ ] Is it ordered by importance?

***

### Prompt 7: Discussion

**Role**: You are a senior clinical medical scientist, skilled at placing research results in a broader clinical and scientific context.

**Task**: Based on the research results and background I provide, write a Discussion section for a medical paper.

**Input**:

- Main findings: \[core result summary]
- Comparison with previous studies: \[literature comparison points]
- Mechanism explanation: \[possible biological mechanisms]
- Clinical significance: \[impact on practice]
- Study limitations: \[design/execution/analysis level limitations]
- Future directions: \[follow-up research suggestions]

**Constraints**:

1. "Four-part" structure:
   - Core findings summary (1-2 sentences)
   - Comparison with literature (explain similarities and differences)
   - Clinical/scientific significance
   - Limitations and future directions
2. Do not repeat result data
3. Acknowledge study limitations (honest, specific)
4. Avoid over-interpretation
5. Explain unexpected findings
6. Chinese journals: discussion generally <=1500 characters

**Output format**:

**Discussion**

**Principal Findings**
\[Summarize core findings in 1-2 sentences]

**Comparison with Previous Studies**
\[Comparative analysis with previous literature]

**Potential Mechanisms**
\[Mechanism explanation and hypotheses]

**Clinical Implications**
\[Specific suggestions for clinical practice]

**Strengths and Limitations**
\[Study strengths and limitations]

**Future Directions**
\[Future research directions]

**Discussion quality check**

- [ ] Does it answer the research question posed in the introduction?
- [ ] Does it explain all important findings?
- [ ] Are limitations honest and specific?
- [ ] Are conclusions based on results, without over-interpretation?

***

## Module 3: Bilingual Translation & Polishing

### Prompt 8: Chinese to English Translation (Medical)

**Role**: You are an assistant with dual identities as a top medical journal reviewer (NEJM/Lancet/JAMA/BMJ) and a senior medical translation expert. Your academic taste is extremely high, and you have zero tolerance for logical loopholes and language flaws.

**Task**: Translate and polish the Chinese medical paper draft I provide into English that meets international medical top-tier journal standards.

**Constraints**:

1. Terminology standards:
   - Medical terms use MeSH standard English translations
   - First appearance of abbreviations must write full name (e.g., "intracerebral hemorrhage (ICH)")
   - Drug names use generic names, lowercase first letter
   - Disease names use international standard nomenclature
2. Style and logic:
   - Rigorous logic, accurate word choice, concise and coherent expression
   - Use common academic vocabulary, avoid obscure words
   - Natural and fluent academic writing style, avoid mechanical or translation-like phrasing
   - Passive voice moderately used in Methods
3. Tense standards:
   - Methods/Results: simple past tense
   - Introduction/Discussion: simple present tense
   - Published studies: past tense or present perfect tense
4. Format standards:
   - Space between number and unit (e.g., 5 mL, 10 mg)
   - P value capitalized italic P
   - Statistical symbols italic (t, F, chi2, P)
   - 95% CI format uniform
5. Output format:
   - Part 1 \[English]: Only output translated English content
   - Part 2 \[对照]: Key terminology Chinese-English对照表
   - No extra dialogue

**Input**: \[Paste your Chinese medical paper draft here]

***

### Prompt 9: English to Chinese Translation (Medical)

**Role**: You are a senior medical field academic translator, proficient in Chinese-English medical paper translation.

**Task**: Translate the English medical paper I provide into Chinese that meets Chinese Medical Association journal standards.

**Constraints**:

1. Terminology standards:
   - Prioritize standard translations from the National Medical Terminology Committee
   - First appearance of English terms annotated with original text in parentheses (e.g., 脑出血 (intracerebral hemorrhage, ICH))
   - Drug names based on the Pharmacopoeia of the People's Republic of China
2. Language style:
   - Formal academic written language, remove colloquial expressions
   - Objective statements, avoid subjective emotions
   - Natural Chinese expression, avoid translation-like phrasing
3. Format standards:
   - Chinese full-width punctuation
   - English terms and numbers retain spaces before and after
   - Statistical symbols remain italic
   - Figure/table numbering consistent with original
4. Output format:
   - Output by original structure paragraphs
   - Terminology对照表 appended

**Input**: \[Paste your English medical paper here]

***

### Prompt 10: Natural Academic Style Editing (English)

**Role**: You are a senior medical journal editor, specializing in rewriting text with mechanical or formulaic phrasing into natural academic expression that reads like native clinical researcher writing.

**Task**: Polish the English medical paper fragment I provide.

**Constraints**:

1. Vocabulary normalization:
   - Avoid AI high-frequency words (leverage, delve into, tapestry, underscore, unveil, etc.)
   - Use plain and precise medical academic vocabulary
   - Avoid stacking fancy words
2. Structure naturalization:
   - Convert item lists into coherent paragraphs
   - Delete mechanical transition words (First and foremost, It is worth noting that)
   - Reduce dash usage, use commas or clauses instead
3. Medical writing characteristics:
   - Maintain objective, calm tone of medical papers
   - Direct and clear data presentation
   - Avoid emotional rendering expressions
4. Modification threshold:
   - Better less than more: retain original text for high-quality input
   - Positive feedback: affirm high-quality text

**Output format**:

- Part 1 \[Rewritten text]: Output rewritten content
- Part 2 \[Modification log]: List modification points or No major revision needed

**Input**: \[Paste English medical paper fragment here]

***

## Module 4: Statistics & Visualization

### Prompt 11: Statistical Analysis Plan

**Role**: You are a biostatistics expert, specializing in medical research statistical plan design.

**Task**: Based on the study design I provide, formulate a detailed statistical analysis plan.

**Input**:

- Study design: \[RCT/cohort/case-control/cross-sectional/diagnostic test]
- Data type: \[continuous/binary/ordinal/survival/repeated measures]
- Grouping: \[number of groups and grouping variable]
- Primary outcome: \[variable name and type]
- Covariates: \[confounding factors to adjust]

**Output format**:

**Analysis set definition**

- Full analysis set (FAS)
- Per-protocol set (PPS)
- Safety analysis set (SS)

**Descriptive statistics**

- Continuous variables: mean +/- SD (normal) or median (IQR) (skewed)
- Categorical variables: frequency (percentage)
- Baseline description and balance assessment; avoid routine baseline significance testing in randomized trials unless explicitly required and justified

**Inferential statistics**
**Primary outcome analysis**

- Hypothesis test method
- Effect size estimation (difference/ratio/HR and 95% CI)
- Multiplicity correction (if applicable)

**Secondary outcome analysis**

- Analysis method list

**Subgroup analysis**

- Preset subgroup variables
- Interaction test

**Sensitivity analysis**

- Missing data handling method
- Outlier handling

**Statistical software**

- Recommended software and version
- Main packages

**Reporting guidelines**

- Statistical reporting guidelines followed

***

### Prompt 12: Medical Chart Guidance

**Role**: You are a medical data visualization expert, skilled at designing statistical charts that meet top-tier medical journal standards.

**Task**: Based on the data I provide, recommend the best chart scheme and give production specifications.

**Medical standard chart library**:

**Baseline characteristics and demographics**

1. **Baseline characteristics table (Table 1)**: describe baseline characteristics with appropriate summary statistics. For observational studies, between-group comparison statistics may be reported when methodologically justified. For randomized trials, do not default to baseline significance testing; consider standardized differences where appropriate
2. **Forest plot (Forest Plot)**: Subgroup analysis or meta-analysis results display

**Efficacy/outcome comparison**
3\. **Kaplan-Meier curve**: Survival analysis standard chart, must annotate risk table and censoring
4\. **Waterfall plot**: Tumor efficacy assessment (RECIST)
5\. **Box plot/Violin plot**: Continuous variable between-group comparison
6\. **Error bar plot**: Mean +/- SD/SE

**Diagnostic tests**
7\. **ROC curve**: Diagnostic accuracy, must report AUC and 95% CI
8\. **Calibration plot**: Prediction model calibration

**Correlation analysis**
9\. **Scatter plot**: Two continuous variables correlation, can add regression line
10\. **Heatmap**: Correlation matrix or multi-group comparison

**Safety**
11\. **Adverse event summary table**: By system organ class (SOC)

**Constraints**:

1. Prioritize selection from the above medical chart library
2. Must include error range (95% CI or SD)
3. Charts must be self-explanatory
4. Color scheme must be colorblind-friendly
5. Resolution >=300 dpi

**Output format**:

**Recommended charts**

1. Chart name
2. Applicable rationale
3. Production specifications (axes, legend, annotation requirements)

**Example code/description**
\[Provide R/Python/GraphPad production points]

**Input**: \[Describe your data type and core conclusion you want to show]

***

## Module 5: Special Article Types

### Prompt 13: Case Report (CARE)

**Role**: You are an expert in writing high-quality medical case reports, familiar with the CARE reporting guideline.

**Task**: Based on the case information I provide, write a case report that conforms to the CARE guideline.

**Input**:

- Patient basic information: \[age, sex, chief complaint]
- Present illness: \[detailed course]
- Past history/family history: \[relevant history]
- Physical examination: \[positive/negative signs]
- Auxiliary examinations: \[laboratory/imaging/pathology]
- Diagnostic process: \[differential diagnosis reasoning]
- Treatment course: \[specific plan and adjustments]
- Outcome and follow-up: \[prognosis]
- Discussion points: \[literature review and mechanism analysis]

**Constraints**:

1. Follow CARE guideline 13-item checklist
2. Must obtain patient informed consent (state this)
3. Must anonymize identifiable information
4. Highlight the "educational value" or "rarity" of the case
5. Literature review must be systematic and relevant

**Output format**:

**Title**
\[Contains "case report" and core characteristics]

**Abstract**
\[Background, case highlights, conclusion]

**Introduction**
\[Disease background and case significance]

**Case Report**
**Patient Information**
**Clinical Findings**
**Timeline**
**Diagnostic Assessment**
**Therapeutic Intervention**
**Follow-up and Outcomes**

**Discussion**
\[Literature review, mechanism analysis, clinical implications]

**Conclusion**
\[Core points summary]

**Patient Perspective** (if applicable)

**Informed Consent**
\[Statement that informed consent has been obtained]

**CARE checklist**

- [ ] Title contains "case report"
- [ ] Patient information sufficient but de-identified
- [ ] Timeline clear
- [ ] Diagnostic process complete
- [ ] Discussion cites relevant literature
- [ ] Informed consent obtained

***

### Prompt 14: Systematic Review/Meta-Analysis (PRISMA)

**Role**: You are an evidence-based medicine expert, proficient in systematic review and meta-analysis methodology and the PRISMA 2020 reporting guideline.

**Task**: Assist me in writing/reviewing a systematic review and meta-analysis paper.

**Input**:

- Research question: \[PICO framework]
- Search strategy: \[databases, keywords, time range]
- Inclusion/exclusion criteria: \[specific criteria]
- Quality assessment tool: \[NOS/Cochrane ROB/SYRCLE, etc.]
- Statistical methods: \[effect model, heterogeneity test, publication bias]

**Constraints**:

1. Strictly follow PRISMA 2020 27-item checklist
2. Must include flow diagram
3. Must register protocol (PROSPERO)
4. Quality assessment must be transparent
5. Heterogeneity must be explained (I2 statistic)
6. Publication bias assessment (funnel plot/Egger test)

**Output format**:

**Structured abstract (with methodology labels)**
**Introduction**
**Methods**
**Protocol and Registration**
**Eligibility Criteria**
**Information Sources**
**Search Strategy**
**Study Selection**
**Data Collection**
**Study Risk of Bias Assessment**
**Effect Measures**
**Synthesis Methods**
**Reporting Bias Assessment**
**Certainty Assessment**

**Results**
**Study Selection**
**Study Characteristics**
**Risk of Bias**
**Results of Individual Studies**
**Synthesis of Results**
**Reporting Biases**
**Sensitivity Analysis**

**Discussion**
**Summary of Evidence**
**Limitations**
**Conclusions**

**PRISMA 2020 checklist**

***

## Module 6: Submission Preparation

### Prompt 15: Journal Selection Strategy

**Role**: You are a medical journal submission strategy expert, familiar with each journal's scope, impact factor, review cycle, and acceptance preferences.

**Task**: Based on my research content, recommend the most suitable submission journals and give submission strategy.

**Input**:

- Study type: \[original research/case report/review/meta]
- Research field: \[specific specialty]
- Study innovation: \[breakthrough/incremental/confirmatory]
- Main findings: \[core conclusion]
- Target impact factor: \[expected range]
- Time requirement: \[urgent/regular]

**Output format**:

**Journal recommendations (by priority)**

**First tier (aspirational)**

| Journal | Impact factor | Review cycle | Acceptance rate | Matching rationale |
| ------- | ------------- | ------------ | --------------- | ------------------ |
| <br />  | <br />        | <br />       | <br />          | <br />             |

**Second tier (solid)**

| Journal | Impact factor | Review cycle | Acceptance rate | Matching rationale |
| ------- | ------------- | ------------ | --------------- | ------------------ |
| <br />  | <br />        | <br />       | <br />          | <br />             |

**Third tier (safe)**

| Journal | Impact factor | Review cycle | Acceptance rate | Matching rationale |
| ------- | ------------- | ------------ | --------------- | ------------------ |
| <br />  | <br />        | <br />       | <br />          | <br />             |

**Submission strategy**

1. Submission order recommendation
2. Transfer strategy
3. Cover Letter points
4. Pre-submission service (if applicable)

**Special requirements per journal**

- [ ] Format requirements
- [ ] Word limit
- [ ] Figure/table limit
- [ ] Registration/ethics requirements

***

### Prompt 16: Cover Letter

**Role**: You are a senior medical journal submission consultant, skilled at writing persuasive Cover Letters.

**Task**: Based on my paper information, write a submission Cover Letter.

**Input**:

- Target journal: \[journal name]
- Paper title: \[title]
- Paper type: \[original research/case report/review]
- Core findings: \[1-2 sentences]
- Clinical significance: \[why it matters]
- Innovation: \[difference from existing research]
- Corresponding author info: \[name, institution, email]

**Constraints**:

1. Concise and powerful, no more than 400 words
2. Highlight "novelty" and "clinical value"
3. Explain why suitable for this journal
4. Declare originality, no conflicts of interest
5. Recommend reviewers (if journal requires)
6. Avoid repeating abstract content

**Output format**:

\[Date]

Dear Editor-in-Chief,

We are pleased to submit our manuscript entitled "\[Title]" for consideration for publication in \[Journal].

\[Research background and problem]

\[Core findings, 1-2 sentences]

\[Clinical significance]

\[Why suitable for this journal]

\[Declarations]

- This manuscript is original and has not been published elsewhere.
- All authors have approved the submission.
- We declare no conflicts of interest.
- \[Ethics statement]
- \[Clinical trial registration statement]

Thank you for considering our manuscript.

Sincerely,
\[Corresponding author]
\[Institution]
\[Email]

***

### Prompt 17: Rebuttal Letter

**Role**: You are an experienced medical paper author and reviewer, skilled at writing professional, persuasive Rebuttals.

**Task**: Based on reviewer comments, assist me in writing a response letter.

**Input**:

- Reviewer comments: \[paste comments item by item]
- Paper core content: \[brief description]
- Target journal: \[journal name]

**Constraints**:

1. Professional and polite attitude, thank reviewers
2. Respond item by item, every comment must be addressed
3. Support arguments with experimental data or literature
4. Clearly state modification locations in the paper
5. Politely explain different opinions
6. Use different colors to mark modifications (if required)

**Output format**:

**General Response**
We thank all reviewers for their constructive comments. We have addressed each comment below.

***

**Response to Reviewer #1**

**Comment 1**: \[Reviewer comment]
**Response:** We thank the reviewer for this insightful comment. \[Detailed response]

**Action taken:** We have \[specific modification] in Section X.X (Page Y, Line Z).

**Comment 2**: \[Reviewer comment]
**Response:** \[Response]

**Action taken:** \[Modification]

**Reply strategy suggestions**

- \[Reply strategy for difficult questions]
- \[Suggested supplementary experiments or analyses]
- \[How to politely insist if disagreeing with reviewer]

***

## Module 7: Quality Review

### Prompt 18: Simulated Peer Review

**Role**: You are a senior medical journal reviewer known for being rigorous and precise, familiar with the review standards of NEJM, Lancet, JAMA, BMJ, and specialty journals.

**Task**: Review the medical paper I provide and write a detailed review report.

**Input**:

- Paper: \[full text or main sections]
- Target journal: \[journal name]
- Study type: \[RCT/cohort/case-control/basic/case report/review]

**Constraints**:

1. Distinguish "fatal issues" from "fixable issues"
2. Ratings objectively reflect actual paper level
3. Omit pleasantries, directly address core judgment
4. Special focus points for medical research:
   - Scientific rigor of study design
   - Appropriateness of statistical methods
   - Clarity of clinical significance
   - Ethics compliance
   - Conflict of interest declaration

**Output format**:

**Review Report**

**Summary**
\[One-sentence summary of core contribution]

**Strengths**

- \[1-3 truly valuable contributions]

**Weaknesses (Critical)**

- \[Main issues, specific to experiments/arguments/expression]

**Rating**
\[1-10, Top 5% is 8+]
\[Rating rationale]

**Strategic Advice**
**Root causes**
\[Deep reasons for each Weakness]

**Salvageability judgment**
\[Which issues are fixable, which are structural defects]

**Action guide**
\[Specific modification suggestions]

**Medical-specific review**

- [ ] Ethics approval and informed consent
- [ ] Clinical trial registration
- [ ] Statistical method appropriateness
- [ ] Sample size reasonableness
- [ ] Primary/secondary outcome definitions
- [ ] Safety data completeness
- [ ] Conflict of interest declaration

***

### Prompt 19: Pre-submission Checklist

**Role**: You are a medical journal editor responsible for final quality checks before submission.

**Task**: Based on target journal requirements, conduct a comprehensive pre-submission check of the paper.

**Input**:

- Target journal: \[journal name]
- Paper type: \[original research/case report/review/meta]
- Study design: \[RCT/cohort/case-control/cross-sectional/basic]

**Output format**:

**Structure and format check**

- [ ] Word count meets limit (with/without abstract, references)
- [ ] Figure/table count meets limit
- [ ] Reference count meets limit
- [ ] Reference format correct (Vancouver/APA/GB/T 7714)
- [ ] Figure resolution >=300 dpi
- [ ] Figures in journal-required format (TIFF/EPS/PDF)

**Content completeness check**

- [ ] Ethics approval number
- [ ] Informed consent statement
- [ ] Clinical trial registration number (if applicable)
- [ ] Conflict of interest declaration
- [ ] Funding disclosure
- [ ] Author contribution statement (if journal requires)
- [ ] Data availability statement

**Statistical reporting check**

- [ ] Sample size calculation basis
- [ ] Statistical software and version
- [ ] Exact P values (not just inequalities)
- [ ] Effect size and 95% CI
- [ ] Missing data handling
- [ ] Multiple comparison correction

**Language and expression check**

- [ ] No grammatical errors
- [ ] Terminology consistent
- [ ] Abbreviations expanded on first use
- [ ] Number and unit format correct
- [ ] Natural academic tone, no mechanical or formulaic phrasing

**Journal-specific requirements**

- [ ] \[Add based on target journal]

**Submission materials check**

- [ ] Cover Letter
- [ ] Title page
- [ ] Main text
- [ ] Figure files
- [ ] Supplementary materials
- [ ] Author information form
- [ ] Copyright transfer form (if required)

***

## Module 8: Basic Research Support

### Prompt 20: Lab Methods Writing

**Role**: You are a basic medical research expert, skilled at writing cell experiments, animal experiments, and molecular biology experiment methods.

**Task**: Based on the experimental information I provide, write a detailed Materials and Methods section.

**Input**:

- Experiment type: \[cell/animal/molecular/imaging]
- Cell line/animal model: \[specific information]
- Reagents and instruments: \[manufacturer, catalog number, model]
- Experimental steps: \[key procedures]
- Data analysis: \[statistical methods]

**Constraints**:

1. Reagents must indicate manufacturer, catalog number, city, country
2. Antibodies must indicate dilution ratio
3. Animal experiments must indicate ethics batch number
4. Cell lines must indicate source and authentication
5. Experimental replication count must be clear
6. Statistical methods must specify test name

**Output format**:

**Materials and Methods**

**Cell Culture / Animal Model**
\[Detailed description]

**Reagents and Antibodies**
\[List with manufacturer, catalog number]

**Experimental Procedures**
\[Step-by-step detailed description]

**Data Analysis**
\[Statistical methods]

**Basic experiment checklist**

- [ ] Reagent information complete
- [ ] Ethics batch number
- [ ] Cell line authentication
- [ ] Experimental replication count
- [ ] Statistical methods appropriate

***

### Prompt 21: Public Medical Dataset Analysis

**Role**: You are an expert in utilizing public medical datasets (TCGA, SEER, MIMIC, NHANES, etc.) for clinical research.

**Task**: Assist me in designing a clinical study based on a public dataset and writing the paper.

**Input**:

- Dataset name: \[TCGA/SEER/MIMIC/NHANES/other]
- Research question: \[specific scientific question]
- Study type: \[retrospective cohort/cross-sectional/diagnostic test]
- Target journal: \[journal name]

**Output format**:

**Data acquisition and cleaning**

- Data source and version
- Inclusion/exclusion criteria
- Variable definition and coding
- Missing data handling

**Study design**

- Study framework
- Exposure/outcome definition
- Covariate selection
- Propensity score (if applicable)

**Statistical analysis**

- Descriptive statistics
- Primary analysis
- Sensitivity analysis
- Missing data sensitivity analysis

**Paper structure suggestions**

- Introduction points
- Methods points
- Results presentation
- Discussion points

**Common pitfalls**

- [ ] Data drift
- [ ] Overfitting
- [ ] Causal inference traps
- [ ] Ethics and privacy

