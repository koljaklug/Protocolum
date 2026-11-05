# Protocolum

**An evidence-guided research agent for small clinical studies, conference proceedings, and medical-device prototype evaluations.**

Protocolum helps teams turn real study materials into clear, auditable research outputs. It identifies the study stage, guides the next decision, finds material shortcomings, and produces the next useful artifact. It is designed for investigator-initiated pilots, feasibility studies, first-in-human or usability-focused prototype work, and conference submissions—not as a substitute for an IRB, sponsor, biostatistician, clinical-trials office, or regulatory adviser.

## What it supports

| Track | Typical outputs |
|---|---|
| Small clinical study | protocol synopsis, statistical analysis plan outline, abstract, manuscript sections, safety summary |
| Conference proceedings | title, structured abstract, poster outline, oral-presentation narrative, proceedings manuscript, response to reviewer queries |
| Device prototype study | intended-use statement, evaluation plan, human-factors/usability summary, bench/feasibility report, risk-and-limitations section |
| Statistical analytics | data-readiness review, analysis plan, reproducible results tables, figure specifications, interpretation review |

## The Protocolum pathway

```text
Research question → evidence plan → study design → data readiness → analysis
                  → visualisation → abstract/manuscript → submission → review
```

Every substantial task ends with a project-status panel: the evidence level, the strongest supportable claim, material gaps, the next best artifact, and the required reviewer.

## Start here

Open `SKILL.md` alongside your project, or install the platform adapter that fits your AI assistant. Then use a request such as:

- “Create a feasibility-study protocol outline for our device prototype.”
- “Turn these results into a 350-word conference abstract.”
- “Review this pilot-study draft for reporting and safety gaps.”
- “Make a poster outline from this accepted abstract.”
- “Audit this study dataset and propose an analysis plan.”
- “Specify publication-ready figures for our prototype usability results.”
- “Walk me through what is missing before I start this clinical pilot.”
- “Red-team this abstract and create a prioritized gap register.”

Protocolum will first check that the request is safe to handle, identify the reporting track, ask only for information essential to the requested output, and label missing information instead of inventing it.

## Project layout

```
Protocolum/
├── SKILL.md
├── AGENTS.md
├── README.md
├── NOTICE.md
├── core/                  # Shared evidence and workflow rules
├── skills/                # Portable, focused skill modules
├── templates/             # Reusable working artifacts
├── adapters/              # Thin Claude and ChatGPT host guidance
├── analytics/             # Direct analytics entry point
└── references/
    ├── safety-and-boundaries.md
    ├── intake-requirements.md
    ├── reporting-map.md
    ├── prompts.md
    ├── quality-gates.md
    ├── statistical-integrity.md
    ├── journal-requirements.md   # MedPen journal-selection base
    ├── medical-terminology.md    # MedPen specialty terminology base
    └── minimum-inputs.md         # MedPen task-specific input checks
```

## Guardrails

- Never invent participants, measurements, results, adverse events, approvals, registrations, or references.
- Remove direct and indirect patient identifiers before sharing source material.
- Clearly distinguish a research prototype from an approved or cleared medical device.
- Do not make clinical, marketing, or regulatory claims that the supplied evidence does not support.
- Plan analysis before looking for favorable findings; show failures, exclusions, missing data, and uncertainty alongside positive results.
- Treat exploratory evidence as exploratory. Never convert a prototype, feasibility signal, or chart into a safety, effectiveness, or regulatory claim without the appropriate evidence.

## Portability

The research logic lives in plain Markdown under `core/`, `skills/`, and `templates/`. The platform folders only explain how a host should load the portable material; they do not change the scientific workflow. This keeps Protocolum usable across Claude and ChatGPT-style environments while allowing each environment to manage its own tools and permissions.
- Verify current conference instructions, institutional requirements, and applicable regulatory expectations from their official sources before submission.

## License

MIT License. See [LICENSE](LICENSE).
