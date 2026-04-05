# BSCECOM18 Research Orchestrator

A staged academic research skill that transforms a bachelor thesis and supporting source archive into structured expert analysis, originality plans, bilingual article blueprints, and polished PhD-level paper drafts.

## Overview

`bscecom18-research-orchestrator` is designed for research projects that begin with an existing thesis, dissertation chapter, seminar paper, or source archive and need to be extended into a stronger academic contribution.

The current default project theme is:

> **The legal digital personality: from a 2019 robots approach to AI in 2026**

The skill preserves the original thematic core of the source work while reframing it for a more current and defensible 2026 research context.

It is especially useful for interdisciplinary projects at the intersection of:

* law
* taxation and fiscality
* automation and artificial intelligence
* labour economics
* social-insurance financing
* governance and legal theory

## What the Skill Does

The skill runs a staged workflow around a thesis and its project materials.

It can:

* inventory and map project sources
* extract the original research question, method, and conclusions
* identify which assumptions remain valid and which are outdated
* run separate expert reviews from multiple disciplinary lenses
* generate originality audits and extension strategies
* produce article blueprints for a PhD-level paper
* write full article drafts in **English and French**
* keep the two final researcher syntheses **independent**, even when they share the same source material and subject

## Core Research Subject

By default, the skill is configured around the shared subject:

> **The legal digital personality: from a 2019 robots approach to AI in 2026**

This means the skill is optimized to explore questions such as:

* How should a 2019 robot-centered legal or tax debate be reframed in 2026?
* What remains analytically valid from earlier robot-tax or robot-personality arguments?
* How should AI systems be treated in legal, fiscal, and governance analysis today?
* Is full legal personality the right framework, or should a narrower legal-digital attribution model be preferred?

## Role Architecture

The skill uses **five role lenses**.

### Expert roles

* **economist expert**
* **fiscality expert**
* **legal personality expert**

These roles do not write the final article. They generate expert inputs, critiques, reframings, and extension ideas.

### Researcher roles

* **researcher agent english**
* **researcher agent french**

These two researcher agents:

* work from the **same expert base**
* share the **same research subject**
* synthesize the expert outputs **independently**
* produce two separate articles, one in English and one in French
* are **not** meant to produce simple translations of each other

## Workflow

The default execution order is:

1. **Intake and source map**
2. **Economist review**
3. **Fiscality review**
4. **legal personality review**
5. **Researcher synthesis (English)**
6. **Researcher synthesis (French)**
7. **Originality and extension planning**
8. **Article blueprint**
9. **Final English LaTeX draft**
10. **Final French LaTeX draft**
11. **Optional PDF rendering**

At each stage, the skill documents:

* input used
* transformation performed
* output produced
* unresolved questions

## Default Outputs

When the user says something like **“run the app”** or provides the thesis plus archive without narrowing the request, the skill returns this bundle:

1. project inventory
2. analysis
3. summary referee
4. academic review
5. originality
6. next step
7. extensions
8. article blueprint
9. researcher-written article draft in English LaTeX
10. researcher-written article draft in French LaTeX

## Input Types

The skill can use the following inputs when available:

* uploaded bachelor thesis PDF
* uploaded project ZIP or extracted source folder
* uploaded notes, draft chapters, or bibliographies
* optional Google Drive documents when explicitly referenced

Typical project materials include:

* original thesis manuscript
* bibliography files
* draft articles
* notes on legal doctrine or tax-policy developments
* source PDFs and reference folders

## Repository Structure

```text
bscecom18-research-orchestrator/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── workflow.md
│   ├── expert-roles.md
│   ├── output-spec.md
│   ├── article-blueprint.md
│   ├── commands.md
│   └── reuse-guide.md
└── assets/
    └── latex/
        └── article-template.tex
```

## Key Files

### `SKILL.md`

Main skill instructions and staged workflow logic.

### `references/workflow.md`

Execution sequence and documentation rules.

### `references/expert-roles.md`

Responsibilities of the macro, fiscality, law, and researcher agents.

### `references/output-spec.md`

Default structure for analysis, originality, blueprint, and final article outputs.

### `references/article-blueprint.md`

Shared subject framing, title patterns, and recommended 20-page architecture.

### `references/commands.md`

Command-style triggers such as `inventory`, `analyse`, `originality`, `article blueprint`, and `draft article`.

### `references/reuse-guide.md`

Guidance for adapting the skill to another thesis or adjacent topic.

### `assets/latex/article-template.tex`

Reusable LaTeX skeleton for article drafting.

## Example Prompts

### Full project run

```text
I uploaded my 2019 bachelor thesis and the full project archive. Run the bscecom18-research-orchestrator end to end on this project. Keep the Swiss framing, update the debate from a 2019 robots approach to AI in 2026, and produce the full staged bundle.
```

### Inventory only

```text
Inventory this project and build a source map. Extract the original research question, hypotheses, method, conclusion, and identify what is outdated by 2026.
```

### Expert analysis only

```text
Analyse this thesis with the macro economist, fiscality expert, and law doctor lenses, then produce independent English and French syntheses.
```

### Blueprint request

```text
Build the article blueprint for the shared subject “The legal digital personality: from a 2019 robots approach to AI in 2026”.
```

### Drafting request

```text
Write both full article drafts in LaTeX. The English and French versions must be independent syntheses, not translations.
```

## Use Cases

This skill is a good fit when you want to:

* upgrade a bachelor thesis into a more publishable paper
* test how a 2019 argument survives in a 2026 AI context
* generate a bilingual academic article package
* separate disciplinary expert review from final article writing
* preserve traceability between original thesis claims and new contributions

## Design Principles

The skill follows several core design principles:

* **the original thesis remains visible**: the workflow explicitly tracks what comes from the source thesis and what is newly added
* **experts and researchers are separated**: the expert roles diagnose and critique, while the researcher roles synthesize and write
* **bilingual outputs are independent**: the English and French researcher agents may converge on substance but should differ in framing, emphasis, and argumentative flow
* **the 2019 to 2026 transition is explicit**: the skill is built to identify continuity, revision, and novelty
* **the writing should remain defensible**: the skill avoids unsupported futurism and forces explicit assumptions

## Recommended Research Questions

The skill is especially strong for projects built around questions such as:

* Should AI receive a limited legal digital personality in 2026?
* How should the legal personality of robots be reframed in the age of AI systems?
* What is the most defensible legal and fiscal architecture for AI-driven production?
* How should social-insurance financing evolve when automation becomes increasingly intangible?

## Reusing the Skill for Other Projects

The skill can be reused for other thesis-based research workflows.

When adapting it:

* keep the staged workflow
* keep the separation between expert roles and researcher roles
* keep the documentation of transformations from source work to extended article
* change the shared subject only when the new project truly requires a different thematic frame

## Current Focus and Limits

This skill is currently optimized for:

* Swiss and European legal-policy reasoning
* AI, taxation, legal personality, and social-insurance questions
* thesis-to-article transformation
* bilingual English/French academic drafting

It is less suited to:

* purely empirical econometrics projects with no legal or policy dimension
* highly technical computer-science research workflows
* non-academic output formats

## Contribution Pattern

A strong output from this skill usually does three things:

1. recovers the logic of the original thesis
2. shows why the 2019 robot framing is incomplete in 2026
3. replaces the narrow earlier framing with a broader and more defensible AI-era legal and fiscal architecture

## Status

This repository contains the reusable skill resources for the BSCECOM18 research workflow.

It is intended for iterative academic development and can be extended with:

* stronger bibliographic resources
* target-journal formatting rules
* citation-style templates
* additional doctrinal or comparative-law references
* rendering scripts for publication-ready PDFs

## License

Add your preferred license here.

## Acknowledgment

Built to support the transformation of thesis-based research into stronger interdisciplinary academic outputs in law, economics, taxation, and AI governance.
