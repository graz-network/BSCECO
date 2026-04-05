# BSCECOM18 Research Orchestrator

BSCECOM18 Research Orchestrator is a reusable academic-research workflow built around David Graz's 2019 bachelor thesis on robot taxation and its 2026 extension toward AI fiscal architecture. The project is designed to help researchers and students transform a source paper and its project materials into structured academic outputs such as summaries, referee reports, originality assessments, extension plans, and article drafts.

The orchestrator is especially suited to projects that begin with an existing thesis, working paper, seminar draft, or dissertation chapter and aim to push it toward a stronger research article.

## Research focus

The core thematic line of the project is the evolution from **robots** to **AI systems** between **2019 and 2026**, with a focus on:

- robot taxation
- AI-enabled automation
- labour share and inequality
- social-insurance financing
- Swiss and comparative fiscal architecture
- legal feasibility and operator-based AI governance

## Objectives

The repository is organized to support four main objectives:

1. **Analyse a source paper rigorously**
2. **Produce reusable academic outputs**
3. **Extend the original research question into a stronger article**
4. **Document the workflow clearly enough for students to understand and reuse it**

## What the orchestrator produces

Depending on the workflow selected, the project can generate:

- academic summary
- referee report
- academic review
- originality assessment
- next-step memo
- extension roadmap
- PhD-level article draft
- LaTeX manuscript
- compiled PDF
- annotated PDF with highlights and comments
- merged output packets combining source article and generated material

## Core intellectual starting point

The project starts from the argument that a literal robot tax is generally weak policy in a small open economy because it is hard to define, hard to administer, and likely to create distortionary incidence effects. The 2026 extension reframes that debate around AI systems, intangible automation, and firm-level fiscal architecture rather than machine-specific taxation.

## Multi-agent architecture

The default orchestrator uses expert roles rather than independent code agents. Each role contributes a specific layer of reasoning.

### 1. Macro economist expert
Focus:
- automation and productivity
- labour share and wages
- incidence and distortion
- macroeconomic modelling
- transition and redistribution effects

Typical questions:
- What happens to labour demand when automation shifts from embodied robots to intangible AI?
- Which tax base is least distortionary in a small open economy?
- How do the results compare with the literature on automation and inequality?

### 2. Fiscality expert
Focus:
- tax-base design
- administrative feasibility
- compliance costs
- social-insurance financing
- VAT, value-added, and firm-level taxation
- international tax coordination

Typical questions:
- Is the proposed tax base observable and enforceable?
- Would a robot tax or AI tax be inferior to broader firm-level or value-added approaches?
- How should fiscal instruments be framed for Switzerland?

### 3. Law doctor
Focus:
- legal coherence
- taxable object definition
- legal personhood debates
- AI governance
- regulatory feasibility
- Swiss and European legal framing

Typical questions:
- Can AI systems realistically be treated as taxable persons?
- What is the legal difference between taxing an object, an operator, and a firm?
- How does the regulatory trend affect fiscal design?

### 4. Researcher agent
Focus:
- synthesis
- final argument design
- article architecture
- final writing
- LaTeX drafting
- output coherence across all stages

This role is the final writing authority. All final article drafting should be consolidated and written by the **researcher agent**.

## Default workflow

The standard end-to-end workflow is:

1. **Ingest source material**
   - bachelor thesis PDF
   - project archive
   - notes, references, and contextual files
2. **Map the original argument**
   - identify question, thesis, method, assumptions, and findings
3. **Generate structured research outputs**
   - summary
   - referee report
   - academic review
   - originality note
   - extension memo
4. **Reframe the research question**
   - move from robot taxation toward AI fiscal architecture where appropriate
5. **Stress-test the identification and policy logic**
   - endogeneity
   - omitted variables
   - external validity
   - counterfactual logic
   - robustness expectations
6. **Build the article blueprint**
   - title
   - abstract
   - literature review
   - theoretical framing
   - empirical or conceptual contribution
   - policy implications
7. **Write the final article**
   - led by the researcher agent
   - output in LaTeX first
   - compile to PDF when required
8. **Document the process for reuse**
   - preserve prompts, structures, and output templates for students

## Repository structure

A recommended repository layout is:

```text
bscecom18-research-orchestrator/
├── README.md
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── article-blueprint.md
│   ├── command-map.md
│   ├── expert-roles.md
│   ├── output-spec.md
│   ├── student-reuse-guide.md
│   └── workflow.md
├── templates/
│   ├── academic-review-template.md
│   ├── extension-plan-template.md
│   ├── originality-template.md
│   ├── referee-report-template.md
│   └── latex-article-template.tex
├── assets/
│   └── latex/
│       └── article-template.tex
├── inputs/
│   ├── pdf/
│   ├── notes/
│   └── archives/
├── outputs/
│   ├── summaries/
│   ├── reports/
│   ├── annotated-pdfs/
│   ├── merged-packets/
│   ├── latex/
│   └── pdf/
└── docs/
    ├── methodology.md
    ├── contribution-map.md
    └── changelog.md
```

## Inputs

The orchestrator is designed to work with:

- uploaded PDF papers
- project ZIP archives
- Google Drive documents
- bundled project context
- prior article drafts
- thesis materials
- bibliography and notes

## Output philosophy

The repository follows five output principles:

1. **Faithfulness first**  
   Do not invent facts missing from the source material.

2. **Constructive critique**  
   Negative comments should always imply a concrete improvement path.

3. **Reusable structure**  
   Outputs should be templated enough for students to reproduce.

4. **Bilingual friendliness where needed**  
   Some workflows may generate English and French versions.

5. **Research escalation**  
   The goal is not just to summarize a bachelor thesis, but to push it toward a stronger article.

## Example command set

Typical orchestrator commands include:

- `analysis`
- `summary`
- `referee_report`
- `academic_review`
- `originality`
- `next_steps`
- `extensions`
- `final_article`
- `pdf_annotations`
- `pdf_resume`

## Suggested usage

### Example 1: thesis-to-article workflow
Use when you want to transform a bachelor thesis into an article draft.

Expected outputs:
- summary
- referee report
- originality memo
- extensions
- final LaTeX article

### Example 2: article evaluation workflow
Use when you want to evaluate a seminar paper or working paper critically before revision.

Expected outputs:
- structured referee report
- academic review
- annotated PDF
- merged article-and-review packet

### Example 3: student learning workflow
Use when the goal is pedagogical.

Expected outputs:
- simplified summary
- contribution map
- critique guide
- explanation of next research steps

## Methodological stance

The orchestrator is designed for rigorous but plain-language academic work. It encourages the user to:

- identify the exact research question
- separate contribution from motivation
- distinguish correlation from causation
- inspect assumptions explicitly
- check for endogeneity and selection bias
- evaluate both statistical and economic significance
- ask whether the chosen method fits the question
- compare the paper against the strongest available benchmark
- propose specific robustness checks rather than vague criticism

## Writing conventions

Preferred style:
- academic
- precise
- constructive
- explicit about uncertainty
- sectioned and reusable
- suitable for LaTeX conversion

Avoid:
- vague praise
- invented data or references
- unsupported causal claims
- generic criticism without a fix

## Recommended README extensions

As the project grows, consider adding:

- a `CONTRIBUTING.md` for student collaborators
- sample input/output pairs
- a reproducibility note
- a bibliography management guide
- a style guide for LaTeX article production

## Quick start

1. Add the source thesis or paper to `inputs/pdf/`
2. Add any ZIP archive or supporting materials to `inputs/archives/`
3. Load the orchestrator skill and relevant templates
4. Run the analysis sequence:
   - summary
   - referee report
   - academic review
   - originality
   - extensions
5. Promote the best extension path into a final article outline
6. Write the article in LaTeX
7. Export or compile the final PDF
8. Save outputs to the appropriate `outputs/` folders

## Intended users

This repository is intended for:

- student researchers
- academic supervisors
- thesis writers
- researchers converting prior work into publishable drafts
- anyone working on automation, taxation, AI governance, or social-insurance financing

## Project origin

The repository is rooted in a 2019 bachelor thesis that evaluated whether robot taxation is desirable, and in a 2026 article draft that translates that question into the era of generative AI, intangible automation, and AI fiscal architecture.

## License

Choose the license that fits your publication and collaboration goals before public release.
