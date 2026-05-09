# MedPen / 捉刀 — Clinical Medical Paper Assistant

<p align="center">
  <b>🩺 AI-Powered Clinical Research Writing Companion</b><br>
  <i>From study design to journal submission — one skill for clinicians and medical researchers</i>
</p>

<p align="center">
  <a href="./README_CN.md">中文</a> ·
  <a href="#-quick-start">Quick Start</a> ·
  <a href="#-features">Features</a> ·
  <a href="#-prompt-library">Prompt Library</a> ·
  <a href="#-quick-start">Quick Start</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-v0.9.0--preview-blue" alt="Version">
  <img src="https://img.shields.io/badge/license-MIT-green" alt="License">
  <img src="https://img.shields.io/badge/language-EN|ZH-brightgreen" alt="Language">
</p>

---

## 📖 Why MedPen?

> **"捉刀"** — In Chinese, it means "to write on behalf of someone" (originating from Cao Cao asking Cui Yan to write for him). It also evokes the surgeon's scalpel, symbolizing precision and professionalism.

Writing clinical research papers is hard. You need to:
- Navigate complex study designs (RCT, cohort, case-control...)
- Follow strict reporting guidelines (CONSORT, STROBE, PRISMA, CARE...)
- Meet journal-specific requirements (NEJM, Lancet, JAMA, BMJ, Stroke, Neurology...)
- Switch between Chinese and English writing seamlessly
- Handle statistical analysis and visualization
- Prepare submission materials (Cover Letter, Rebuttal...)

**MedPen** is a comprehensive AI skill that guides you through the entire workflow — from study design to journal submission — with **21 specialized prompts** tailored for clinical medicine.

---

## ✨ Features

### 🎯 Complete Research Workflow Coverage

| Stage | Prompts | What It Does |
|-------|---------|--------------|
| **Study Design** | #1-2, #11 | RCT/cohort/case-control design, sample size calculation, statistical planning |
| **Paper Writing** | #3-7, #13-14, #20 | Structured abstracts, IMRaD sections, case reports, systematic reviews |
| **Translation & Polishing** | #8-10 | Chinese↔English translation, natural academic style editing, tone refinement |
| **Statistics & Visualization** | #11-12 | Analysis plan design, medical chart recommendations (KM curves, forest plots...) |
| **Submission Prep** | #15-17, #19 | Journal selection, Cover Letter, pre-submission checklist |
| **Peer Review Response** | #17 | Rebuttal letter writing, reviewer comment handling |
| **Quality Review** | #18-19 | Simulated peer review, submission checklist |
| **Basic Research** | #20-21 | Lab methods writing, public dataset analysis (TCGA, SEER, MIMIC...) |

### 🌍 Bilingual Support

- **English → Chinese**: Translate papers for domestic journals (中华医学杂志, etc.)
- **Chinese → English**: Translate drafts for international journals (NEJM, Lancet, etc.)
- **Natural Academic Style Editing**: Refine drafts into fluent, native-level academic expression

### 📋 Medical Reporting Guidelines

Built-in compliance with international standards:
- **CONSORT 2025** — Randomized controlled trials
- **STROBE** — Observational studies
- **PRISMA 2020** — Systematic reviews & meta-analyses
- **CARE** — Case reports
- **TRIPOD** — Prediction models
- **STARD** — Diagnostic accuracy studies

### 🏥 Journal Coverage

MedPen provides writing guidance compatible with a broad spectrum of medical journals, from general medicine top-tier publications to specialized clinical and basic research venues across all medical disciplines. The underlying principles of structured reporting, ethical compliance, and statistical transparency are universally applicable, while specific formatting requirements can be adapted to any target journal.

---

## 🚀 Quick Start

### For Trae / OpenClaw Users

1. **Clone** this repository:
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **Copy** the skill folder to your skills directory:
```bash
# Trae
cp -r MedPen ~/.trae/skills/

# OpenClaw
cp -r MedPen ~/.openclaw/skills/
```

3. **Restart** your IDE or send `/reload`

4. **Start using** — just say:
   - *"Help me design a clinical study"* → triggers Prompt #1
   - *"Translate my Chinese draft to English"* → triggers Prompt #8
   - *"I have a draft, help me prepare for submission"* → triggers sub-flow: #15→#16→#19
   - *"Help me reply to reviewers"* → triggers Prompt #17

### For Cursor Users

1. **Clone** this repository:
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **Copy** the `.cursor/rules.md` file (if available) or open `references/prompts.md` directly in Cursor's composer/chat.

3. **Start using** — mention the prompt number or describe your task in natural language.

### For Claude Code Users

1. **Clone** this repository:
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **Copy** skill folders to your Claude Code skills directory:
```bash
# macOS / Linux
cp -r MedPen ~/.claude/skills/

# Windows (PowerShell)
cp -r MedPen "$env:USERPROFILE\.claude\skills\"
```

3. **Start using** — Claude Code will auto-detect the skill based on your request.

### For GitHub Copilot Users

1. **Clone** this repository:
```bash
git clone https://github.com/Neuro-S/MedPen.git
```

2. **Copy** `.github/copilot-instructions.md` (if available) to your repository or reference `references/prompts.md` in Copilot Chat.

3. **Start using** — describe your task in Copilot Chat.

### For Manual Use (Any AI Tool)

1. Open [`references/prompts.md`](./references/prompts.md)
2. Copy the Prompt you need
3. Paste into Claude, ChatGPT, Cursor, or any AI assistant
4. Fill in your content and run

---

## 📋 Prompt Library

### Module 1: Study Design & Protocol

| # | Prompt | Trigger |
|---|--------|---------|
| 1 | Clinical Study Design Consultation | "Help me design a study" |
| 2 | Sample Size Calculation | "Calculate sample size" |

### Module 2: Structured Paper Writing

| # | Prompt | Trigger |
|---|--------|---------|
| 3 | Structured Abstract | "Write an abstract" |
| 4 | Introduction | "Write an introduction" |
| 5 | Methods | "Write methods section" |
| 6 | Results | "Write results section" |
| 7 | Discussion | "Write discussion" |

### Module 3: Bilingual Translation & Polishing

| # | Prompt | Trigger |
|---|--------|---------|
| 8 | Chinese → English (Medical) | "Translate to English" |
| 9 | English → Chinese (Medical) | "Translate to Chinese" |
| 10 | Natural Academic Style Editing | "Polish academic style" |

### Module 4: Statistics & Visualization

| # | Prompt | Trigger |
|---|--------|---------|
| 11 | Statistical Analysis Plan | "Design statistical analysis" |
| 12 | Medical Chart Guidance | "Recommend charts/figures" |

### Module 5: Special Article Types

| # | Prompt | Trigger |
|---|--------|---------|
| 13 | Case Report (CARE) | "Write a case report" |
| 14 | Systematic Review (PRISMA) | "Write a systematic review" |

### Module 6: Submission Preparation

| # | Prompt | Trigger |
|---|--------|---------|
| 15 | Journal Selection Strategy | "Recommend journals" |
| 16 | Cover Letter | "Write a cover letter" |
| 17 | Rebuttal Letter | "Reply to reviewers" |

### Module 7: Quality Review

| # | Prompt | Trigger |
|---|--------|---------|
| 18 | Simulated Peer Review | "Review my paper" |
| 19 | Pre-submission Checklist | "Check before submission" |

### Module 8: Basic Research Support

| # | Prompt | Trigger |
|---|--------|---------|
| 20 | Lab Methods Writing | "Write lab methods" |
| 21 | Public Dataset Analysis | "Analyze public dataset" |

---

## 📁 Project Structure

```
MedPen/
├── README.md              # This file (English)
├── README_CN.md           # Chinese version
├── LICENSE                # MIT License
├── SKILL.md               # Lightweight task router
├── .gitignore             # Git ignore rules
├── docs/                  # Documentation
│   ├── USAGE.md           # Detailed usage guide
│   ├── ROADMAP.md         # Future development roadmap
│   └── images/            # Screenshots / diagrams
└── references/            # Core rules and prompt library
    ├── safety-and-compliance.md
    ├── minimum-inputs.md
    ├── quality-gates.md
    ├── statistical-anti-misuse.md
    ├── journal-requirements.md
    ├── medical-terminology.md
    └── prompts.md
```

---

## 🎯 Sub-Flow Quick Entry

You don't need to start from the beginning. Jump directly to any sub-flow:

| Sub-Flow | Trigger Statement | Prompt Chain |
|----------|-------------------|--------------|
| **Translate → Submit** | "I have a Chinese draft, help me translate and prepare for submission" | #8 → #10 → #15 → #16 → #19 |
| **Translate Only** | "Help me translate/polish this paper" | #8 or #9 or #10 |
| **Submission Only** | "Help me prepare submission materials" | #15 → #16 → #19 |
| **Rebuttal Only** | "Help me reply to reviewers" | #17 |
| **Review Only** | "Help me review this paper" | #18 or #19 |
| **Statistics Only** | "Help me design statistical analysis" | #11 → #12 |
| **Case Report Only** | "Help me write a case report" | #13 |
| **Systematic Review Only** | "Help me write a systematic review" | #14 |

---

## 🛡️ Safety Boundaries

- ❌ Never fabricate patient data, results, or statistics
- ❌ Never forge ethics approval numbers or trial registration IDs
- ❌ Never invent references or citations
- ✅ All AI-generated content must be verified by the author
- ✅ Clinical decisions should not rely solely on AI suggestions
- ✅ Patient information must be de-identified

---

## 🔮 Extension Roadmap

MedPen is designed for future expansion. Planned modules:

| Module | Feature | Tech Stack |
|--------|---------|------------|
| #9 | Reference Management (auto-formatting, DOI lookup) | Python + Crossref/PubMed API |
| #10 | Medical Data Preprocessing (Table 1 auto-generation) | Python/R |
| #11 | Auto Chart Generation (KM curves, forest plots...) | Python/R |
| #12 | Reporting Guideline Compliance Check | Python rule engine |
| #13 | Journal Format Auto-Adaptation | Python + journal templates |
| #14 | Medical Terminology Auto-Check | Python + MeSH dictionary |
| #15 | Public Dataset Interface (SEER, MIMIC, TCGA) | Python + dataset APIs |

See [docs/ROADMAP.md](./docs/ROADMAP.md) for details.

---

## 🤝 Contributing

Contributions are welcome! You can:

1. **Submit Issues**: Report bugs or suggest new features
2. **Submit PRs**: Improve existing prompts or add new ones
3. **Share Cases**: Submit usage examples and best practices

### Contribution Workflow

```bash
# 1. Fork this repository
# 2. Create a branch
git checkout -b feature/your-feature

# 3. Commit changes
git commit -m "Add: new prompt for XXX"

# 4. Push to branch
git push origin feature/your-feature

# 5. Create Pull Request
```

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

You are free to:
- ✅ Use, modify, and distribute
- ✅ Use for commercial purposes
- ✅ Use for academic research

Requirement: Retain the original copyright notice and license declaration.

---

## 🙏 Acknowledgments

- Inspired by [awesome-ai-research-writing](https://github.com/Leey21/awesome-ai-research-writing)
- Referenced [research-writing-skill](https://github.com/alfonso0512/research-writing-skill)
- Referenced [academic-writing-skills](https://github.com/bahayonghang/academic-writing-skills)
- Built for clinicians, medical researchers, and graduate students worldwide

---

<p align="center">
  <b>MedPen / 捉刀</b> — Write with precision, publish with confidence.
</p>
