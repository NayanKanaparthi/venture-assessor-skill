# Venture Assessor Skill

An evidence-first Claude Skill for evaluating startup ideas through structured market research, competitor analysis, beachhead market selection, BHM TAM sizing, validation planning, and GTM hypothesis generation.

This skill is built for founders, operators, researchers, venture studios, startup advisors, and innovation teams who want to pressure-test an idea before spending months building in the wrong direction.

---

## What this is

**Venture Assessor Skill** is a custom Claude Skill designed to help founders move from a vague idea or problem statement to a structured founder-grade decision memo.

Instead of producing generic market research, this skill follows a disciplined workflow:

- frames the problem clearly
- separates assumptions from evidence
- identifies who is actually facing the problem
- maps pain points and current alternatives
- analyzes direct, indirect, and status-quo competitors
- narrows to a **beachhead market**
- estimates **BHM TAM**
- proposes validation experiments
- suggests a first-pass GTM hypothesis
- ends with a clear verdict and next steps

This is not a "magic yes/no startup predictor."
It is a structured decision-support system that helps founders think better, research faster, and validate more intelligently.

---

## Why this exists

A lot of early-stage startup work goes wrong for predictable reasons:

- the problem is too vaguely defined
- the market is too broad
- competitor analysis is shallow
- TAM is inflated and meaningless
- research is mistaken for validation
- the founder builds before talking to customers
- GTM assumptions are made too early and too loosely

This skill is designed to reduce those mistakes.

It compresses weeks of messy early-stage diligence into a more rigorous, repeatable workflow while keeping one important principle intact:

> Secondary research is useful.  
> It is not the same as validation.

The skill is built to keep that distinction explicit.

---

## Who this is for

This skill is useful for:

- founders evaluating a new startup idea
- startup teams exploring a pivot
- incubator / accelerator participants
- venture studio operators
- consultants doing early-stage opportunity assessment
- product strategists exploring new markets
- students or researchers working on venture discovery

It is especially useful when the input is still rough, such as:

- "I have an idea around AI for healthcare admin workflows"
- "I think freelancers struggle with taxes, can you assess this?"
- "Help me evaluate whether this B2B SaaS concept is worth pursuing"
- "Pressure-test this startup thesis and tell me what to validate next"

---

## What it outputs

The skill produces a structured founder decision memo with sections such as:

1. Executive Summary
2. Problem Statement
3. Evidence vs Assumptions
4. Market Segmentation Options
5. Recommended Beachhead Market
6. Pain-Point Analysis
7. Competitor and Status-Quo Landscape
8. BHM TAM Estimate
9. Validation Plan
10. GTM Hypothesis
11. Business Model Options
12. Risks, Unknowns, and Kill Criteria
13. Final Verdict

The output is designed to support founder decision-making, not just generate a research dump.

---

## Core methodology

This skill follows an evidence-first workflow influenced by disciplined entrepreneurship, customer discovery, market segmentation logic, pain-point analysis, and validation-first startup thinking.

At a high level, it works like this:

### 1. Problem Framing
The skill rewrites a vague idea into a concrete, testable problem statement.

### 2. Evidence Mapping
It distinguishes:

- what the founder believes
- what public signals suggest
- what competitors indicate
- what still requires direct validation

### 3. Market Segmentation
It generates multiple possible market segments, then narrows them using practical filters such as urgency, accessibility, willingness to pay, and strategic fit.

### 4. Pain Analysis
It identifies the real pain points, current workarounds, and why existing solutions may be incomplete or unsatisfying.

### 5. Competitor and Status-Quo Mapping
It evaluates:

- doing nothing
- manual workarounds
- adjacent substitutes
- direct competitors
- incumbent bundles / platforms

### 6. Beachhead Selection
It selects a narrow first market to focus on rather than staying broad and abstract.

### 7. BHM TAM Estimation
It sizes the **beachhead market first**, instead of jumping into vanity TAM logic.

### 8. Validation Design
It proposes concrete next steps such as:

- PMR interviews
- observation
- concierge tests
- saleable concierge
- paid pilots
- low-fidelity offers

### 9. GTM Hypothesis
It suggests a practical first path to market based on the selected segment.

### 10. Final Verdict
It ends with a recommendation such as:

- pursue
- pursue cautiously
- validate before building
- pivot
- pause / kill

---

## Important principles and guardrails

This skill is designed around a few non-negotiable rules:

- **Research is not validation**
- **A market is not "everyone who could benefit"**
- **A startup only becomes a business when someone pays**
- **TAM should not be used as fantasy theater**
- **The status quo is a real competitor**
- **Confidence must be tied to evidence quality**
- **A founder should usually start with one beachhead market**
- **If the market is multi-sided, each side must be treated separately**

---

## Glossary

| Term | Definition |
|------|------------|
| **BHM** | Beachhead Market — the narrow, focused first market you pursue. |
| **PMR** | Primary Market Research — direct customer discovery through interviews, observation, and real-world interaction. |
| **MVBP** | Minimum Viable Business Product — the smallest offer that delivers value and generates learning, such as a saleable concierge, paid pilot, or highly manual service-backed solution. |
| **TAM** | Total Addressable Market — the total economic opportunity. In this skill, **BHM TAM** means the addressable market for the **beachhead only**, not the entire broad industry. |

---

## Repository structure

```
venture-assessor-skill/
├── SKILL.md
├── README.md
└── research_refs/
    ├── methodology/
    │   ├── disciplined_entrepreneurship_core.txt
    │   ├── problem_framing_rules.txt
    │   ├── beachhead_selection_rules.txt
    │   ├── tam_rules.txt
    │   ├── evidence_scoring_rubric.txt
    │   ├── source_selection_map.txt
    │   └── live_research_rules.txt
    ├── analysis/
    │   ├── pain_point_taxonomy.txt
    │   ├── competitor_mapping_framework.txt
    │   ├── business_model_framework.txt
    │   ├── validation_and_gtm_framework.txt
    │   └── decision_rubric.txt
    ├── templates/
    │   ├── founder_input_template.md
    │   ├── output_report_template.md
    │   ├── pmr_interview_guide_template.md
    │   └── validation_experiment_template.md
    └── examples/
        ├── anti_patterns.txt
        └── gold_examples.txt
```

### How the skill is structured

The main entry file is **SKILL.md**.

That file defines:

- the skill name
- the description / trigger
- the objective
- the required context
- the step-by-step SOP
- guardrails
- update logic
- required reference files

The supporting files under `research_refs/` act as the methodology layer.
They help keep the main skill clean and modular, rather than stuffing all logic into one giant prompt.

---

## Installation

### Option 1: Upload into Claude as a custom Skill

If your Claude environment supports custom skill uploads:

1. Clone this repository
2. Ensure the folder contains `SKILL.md` at its root
3. Zip the entire folder
4. Upload that ZIP through Claude's custom Skills interface

**Important:**

- `SKILL.md` must start with valid YAML frontmatter
- The ZIP should contain the skill folder with `SKILL.md` inside it
- Supporting reference files should remain in their relative paths

### Option 2: Use as a reference framework

Even without direct skill upload support, you can still use this repository as:

- a prompt-system design reference
- a reusable venture-evaluation SOP
- a structured founder research framework
- a methodology pack for other agent systems

---

## How to use

Give the skill any of the following:

- a startup idea
- a problem statement
- a market opportunity
- a product concept
- a founder hunch
- a rough venture thesis
- a category you want to explore

### Example prompts

**Example 1:** Evaluate this idea: an AI copilot for independent therapists to automate admin workflows, insurance paperwork, and client follow-up. I want to know if this is worth pursuing.

**Example 2:** Pressure-test this startup thesis: freelancers and solo creators need a better way to manage taxes, cash flow, and business compliance.

**Example 3:** Do market research and validation planning for a B2B SaaS product that helps restaurant chains reduce food waste through predictive inventory recommendations.

**Example 4:** I have a rough idea around AI-powered scholarship guidance for international students. Help me determine the beachhead market, competitors, and what I should validate first.

---

## What makes this different from a normal prompt

This repository is not just "a really long prompt."

It is a structured skill with:

- a defined trigger
- a clean SOP
- modular methodology files
- evidence scoring
- explicit output templates
- validation-first logic
- guardrails against founder delusion
- decision-oriented output

It is designed to behave more like an operating framework than a one-off chat instruction.

---

## Confidence and evidence

One of the most important parts of this skill is that it does not treat all conclusions equally.

The final confidence level should depend on the quality of evidence.

| Level | When to use |
|-------|-------------|
| **High confidence** | Use only when the key assumptions are supported by strong signals and at least some direct or behavior-level evidence. |
| **Medium confidence** | Use when secondary research is strong and internally consistent, but direct validation is still missing or incomplete. |
| **Low confidence** | Use when the thesis is still largely speculative, signal quality is weak, or evidence is contradictory. |

This is intentional.
The goal is to help founders think clearly, not create false certainty.

---

## Multi-sided markets

If the opportunity involves a multi-sided market, the skill should treat each side separately.

Examples:

- buyers and sellers
- creators and audiences
- patients and providers
- merchants and consumers
- operators and end beneficiaries
- advertisers and users

In those cases, segmentation, pain analysis, and value logic should be done per side before choosing the beachhead logic.

---

## What this skill does well

It is strong at:

- turning vague ideas into structured problem statements
- quickly organizing early-stage research
- surfacing likely market and workflow patterns
- mapping status quo and competitor alternatives
- narrowing a broad opportunity into a more focused wedge
- exposing what still needs PMR
- proposing smarter next experiments
- giving founders a cleaner decision framework

## What this skill does not do

It does not:

- prove product-market fit
- replace real customer interviews
- guarantee willingness to pay
- guarantee TAM accuracy
- replace judgment from experienced operators
- eliminate the need for PMR
- guarantee that a startup is "worth pursuing" in absolute terms

This skill accelerates thinking and structure.
It does not replace the real-world work of validation.

---

## Suggested workflow for founders

A strong way to use this skill is:

**Round 1:** Use the skill with your raw idea to get problem framing, segments, likely competitors, initial beachhead, and validation plan.

**Round 2:** Conduct PMR: 10 to 20 interviews, observation where possible, notes on actual behaviors, pains, and language.

**Round 3:** Run the skill again using your PMR findings.

At that point, the memo should become much more useful and grounded because the skill now has direct evidence to work with.

### Example founder use cases

**Founder with a vague idea:** "I think there's a big opportunity in AI for legal ops."
Use the skill to turn that into: which legal workflow, which user, which pain, which market slice, which incumbent alternatives, what to validate first.

**Founder choosing among multiple ideas:** Use the skill to evaluate 3 to 5 ideas with the same structure and compare urgency, accessibility, market wedge, evidence quality, and validation difficulty.

**Team considering a pivot:** Use the skill to re-segment the market and test whether a narrower beachhead may be more viable.

---

## Limitations

This skill depends heavily on:

- the quality of the founder's input
- availability of current web research
- availability of PMR findings
- whether the underlying runtime supports file loading and live research
- whether the environment allows memory or example updates

If the runtime does not support live web research, outputs should be treated as lower-confidence and methodology-driven only.

---

## Roadmap ideas

Possible future improvements:

- stronger source-tiering and citation logic
- support for internal PMR transcript ingestion
- startup database connectors
- CRM or spreadsheet inputs
- better B2B buying-center analysis
- vertical-specific variants
- scoring dashboards
- auto-generated PMR interview scripts by segment
- investor memo mode
- venture studio comparison mode

---

## Contributing

Contributions are welcome if they improve:

- methodological clarity
- practical founder usefulness
- framework rigor
- better examples
- stronger anti-pattern detection
- clearer templates
- better packaging for custom skill runtimes

If you contribute, keep the skill aligned with these principles:

- evidence first
- decision useful
- founder practical
- narrow where needed
- honest about uncertainty

---

## Credits

This skill is inspired by disciplined entrepreneurship, customer discovery, primary market research, startup validation thinking, and practical founder decision-making frameworks.

It is designed as an operational tool for founders who want more rigor before building.

**Author:** Built by [Nayan Kanaparthi](https://github.com/NayanKanaparthi).
