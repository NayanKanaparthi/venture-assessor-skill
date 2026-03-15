---
name: venture-assessor
description: Evaluate startup ideas with evidence-first problem framing, market research, competitor mapping, beachhead selection, BHM TAM, validation design, GTM options, and a verdict.
---

# Venture Assessor

## Overview

Use this skill when a founder wants to evaluate, validate, research, compare, or pressure-test a startup idea, hunch, problem statement, product concept, market opportunity, or early venture thesis.

This skill is for:
- problem validation
- market research
- customer and market segmentation
- pain-point analysis
- competitor and status-quo analysis
- beachhead market selection
- BHM TAM estimation
- validation experiment design
- willingness-to-pay exploration
- initial GTM planning
- go / no-go style founder decision memos

This skill is **not** a substitute for real customer discovery or proof of willingness to pay. It is an evidence-first decision-support workflow that compresses desk research, structures founder thinking, and tells the user what must be validated next.

## Objective

Produce a founder-grade decision memo that helps the user determine whether an idea is worth pursuing, for which narrow market first, under what assumptions, with what evidence, against which alternatives, and with what next experiments.


## Core Terms

- **BHM**: beachhead market — the narrow, focused first market you pursue.
- **PMR**: primary market research — direct customer discovery through interviews, observation, and related firsthand learning.
- **MVBP**: minimum viable business product — the smallest offer that delivers value and generates learning, such as a saleable concierge test or paid pilot.
- **TAM**: total addressable market. In this skill, **BHM TAM** means the addressable market for the beachhead market only.

## Skill Root and Runtime Contract

- Treat the directory containing this `SKILL.md` file as the **skill root**.
- Resolve every relative file path from the skill root, never from the user's project root.
- “Load a reference file” means: read the file contents before analysis and use them as methodology constraints.
- Methodology files constrain reasoning. Template files constrain output shape. Example files refine pattern quality. None of them replace live facts.
- If live web research is unavailable, proceed using user input plus local methodology files only, label all current-state claims as lower confidence, and state that fresh market verification is still needed.
- If optional MCP or equivalent connectors are unavailable, continue without them and explicitly flag which proprietary inputs are missing.
- If the skill directory is read-only, do not fail the run. Instead, emit a **Suggested Memory Update** block so a human can copy successful patterns into `research_refs/examples/gold_examples.txt` or recurring failures into `research_refs/examples/anti_patterns.txt` manually.

## Connectors and Tools

Preferred:
- live web research or web search for current market, competitor, pricing, adoption, funding, and regulatory signals
- file-reading access to the installed skill directory

Optional:
- MCP or equivalent connectors for CRM notes, PMR transcripts, internal memos, proprietary spreadsheets, customer lists, and market databases

## Reference Files to Load

Load these files before analysis:

- `research_refs/methodology/source_selection_map.txt`
- `research_refs/methodology/disciplined_entrepreneurship_core.txt`
- `research_refs/methodology/problem_framing_rules.txt`
- `research_refs/methodology/live_research_rules.txt`
- `research_refs/methodology/evidence_scoring_rubric.txt`
- `research_refs/methodology/beachhead_selection_rules.txt`
- `research_refs/methodology/tam_rules.txt`
- `research_refs/analysis/pain_point_taxonomy.txt`
- `research_refs/analysis/competitor_mapping_framework.txt`
- `research_refs/analysis/validation_and_gtm_framework.txt`
- `research_refs/analysis/business_model_framework.txt`
- `research_refs/analysis/decision_rubric.txt`
- `research_refs/templates/founder_input_template.md`
- `research_refs/templates/output_report_template.md`
- `research_refs/templates/pmr_interview_guide_template.md`
- `research_refs/templates/validation_experiment_template.md`
- `research_refs/examples/anti_patterns.txt`
- `research_refs/examples/gold_examples.txt`

## Workflow

### Step 1: Parse and Plan
1. Read the user's request carefully.
2. Determine whether the input is:
   - a raw hunch
   - a problem statement
   - a startup idea
   - an existing product concept
   - a category or market opportunity
   - a startup already in motion that needs pressure-testing
3. Extract all available context:
   - end-user hypothesis
   - economic-buyer hypothesis
   - problem hypothesis
   - current workaround or alternative
   - geography, industry, or regulatory scope
   - founder constraints
   - existing evidence or traction
4. Separate the starting context into four buckets:
   - founder-supplied facts
   - founder assumptions
   - external facts that must be researched
   - open unknowns
5. Build an internal plan covering:
   - problem framing
   - evidence map
   - market segmentation
   - pain-point analysis
   - competitor and status-quo mapping
   - beachhead selection
   - BHM TAM
   - validation design
   - GTM hypothesis
   - verdict
6. Ask only the minimum clarifying questions required. If the task can proceed with explicit assumptions, proceed.

### Step 2: Context Retrieval
1. Load all required reference files.
2. Treat `research_refs/methodology/disciplined_entrepreneurship_core.txt` as the overarching lens for the full analysis: customer understanding over founder certainty, broad-to-narrow segmentation, one beachhead when possible, and paying-customer logic over narrative.
3. Use `source_selection_map.txt` to decide which frameworks are core, selective, or excluded.
4. Use live web research for:
   - current competitors
   - market signals
   - adoption trends
   - current pricing
   - regulatory or policy context
   - technology maturity
   - recent company activity
5. Use optional connectors only when they materially improve the evidence base, such as:
   - CRM notes
   - prior PMR interviews
   - internal founder notes
   - proprietary spreadsheets or datasets
6. Build an evidence map before synthesis:
   - user facts
   - source-backed facts
   - behavioral proxies
   - inferred hypotheses
   - unresolved unknowns
7. If source quality is weak, say so explicitly.

### Step 3: Execution and Variation
Generate the analysis in the following sequence.

#### 3A. Problem Framing
1. Rewrite the founder's input into a concrete problem statement using the problem framing rules.
2. If the input is vague, generate **3 to 5 problem-framing variations**.
3. For each variation, identify:
   - who has the problem
   - what job, workflow, or outcome is affected
   - current workaround
   - why the workaround is insufficient
   - observable impact
   - likely economic or behavioral consequence

#### 3B. Market Segmentation
1. Brainstorm a broad market universe first.
2. Expand to at least 6 candidate segments when possible.
3. For multi-sided markets, segment each side separately before narrowing. Do not collapse buyers, users, suppliers, creators, advertisers, operators, or beneficiaries into one generic segment unless the pains, buying logic, and adoption path truly overlap.
4. For multi-sided markets, identify which side is most critical or hardest to win first, and state whether the beachhead should be chosen on one side first or on a tightly defined combined interaction.
5. Narrow to the best 3 to 5 candidate segments or side-specific segment combinations.
6. For each segment, provide:
   - end user
   - economic buyer
   - side of the market if multi-sided
   - job or use case
   - pains and benefits
   - accessibility
   - likely budget or willingness to pay
   - major adoption constraints
7. If useful, generate **3 segment-prioritization paths**:
   - urgency-first
   - accessibility-first
   - strategic-leverage-first

#### 3C. Pain-Point Analysis
1. Classify the pains using the pain taxonomy.
2. Rank the pain by:
   - severity
   - frequency
   - urgency
   - cost
   - emotional burden
   - operational burden
3. Estimate the delta between the current state and an improved state.
4. Identify which pains are interesting but not commercially meaningful.

#### 3D. Competitor and Status-Quo Analysis
1. Always map five layers:
   - doing nothing
   - manual workaround
   - adjacent substitute
   - direct competitor
   - incumbent bundle or platform
2. For each major alternative, assess:
   - job solved
   - target user or buyer
   - strengths
   - weaknesses
   - switching friction
   - why the market still tolerates it
   - wedge opportunity
3. If the space is crowded, generate **3 positioning angles**:
   - feature wedge
   - workflow wedge
   - buyer wedge

#### 3E. Beachhead Market Selection
1. Score the top candidate segments using the beachhead rules.
2. Recommend one primary beachhead market.
3. If two options are genuinely close, generate **3 ranked beachhead options** with explicit tradeoffs.
4. Never stay broad when a focused entry market can be chosen.

#### 3F. BHM TAM Estimation
1. Estimate the number of end customers in the chosen beachhead.
2. Estimate the annual revenue per customer to solve the problem.
3. Multiply the two to estimate BHM TAM.
4. Show assumptions clearly.
5. Run a sanity check and highlight confidence limits.
6. Avoid generic TAM/SAM/SOM theater unless used only as a secondary cross-check.

#### 3G. Validation and GTM Hypothesis
1. Identify the top assumptions that must be tested next.
2. Generate:
   - a PMR interview plan
   - a low-fidelity or mockup test
   - a concierge or saleable-concierge test when relevant
   - a paid pilot suggestion when relevant
3. Generate **3 GTM options** when useful:
   - founder-led outbound wedge
   - channel or partner wedge
   - content or community wedge
4. Recommend one first-pass GTM path tied to the chosen beachhead.
5. Suggest business model candidates only after the beachhead and pain logic are credible.

#### 3H. Draft Verdict
1. Produce a draft verdict using the decision rubric.
2. Set confidence by cross-referencing the verdict with `research_refs/methodology/evidence_scoring_rubric.txt`:
   - use **High confidence** only when the core recommendation is supported by strong source quality and at least Tier 3 evidence on the key assumptions, or Tier 4 where payment behavior is central
   - use **Medium confidence** when secondary evidence is solid and there is some Tier 2 or Tier 3 support, but major unknowns remain
   - use **Low confidence** when the thesis is still mostly Tier 0 to Tier 1, when evidence is contradictory, or when critical tools and fresh sources are unavailable
3. Include:
   - recommendation category
   - confidence level
   - strongest evidence tier
   - strongest evidence
   - biggest unknowns
   - fastest next experiments
   - kill criteria
4. Distinguish clearly between:
   - what is supported
   - what is inferred
   - what must still be validated through real customer behavior or payment

### Step 4: Human-in-the-Loop Review
Pause before finalization and present structured choices when ambiguity exists.

1. Present **3 to 5 options** for one or more of:
   - problem framing
   - beachhead market
   - positioning angle
   - validation path
   - GTM path
2. Use a clear selection format such as:

```text
Choose one problem framing:
[ ] A
[ ] B
[ ] C

Choose one beachhead:
[ ] Segment 1
[ ] Segment 2
[ ] Segment 3
```

3. Invite the user to:
   - choose one option
   - combine two options
   - edit an option
   - ask for one more iteration
4. If the user does not choose, proceed with the top-ranked option and clearly say so.

### Step 5: Finalization
1. Produce the final report using `research_refs/templates/output_report_template.md`.
2. Keep the output analytical, specific, actionable, and honest about uncertainty.
3. End with:
   - a clear verdict
   - immediate next actions
   - missing evidence
   - what would change the recommendation
4. If the environment is writable and the user strongly approves the result, save a distilled pattern to `research_refs/examples/gold_examples.txt`.
5. If the environment is read-only, emit a **Suggested Memory Update** block instead.

## Strict Rules and Guardrails

### Must Do
- Always separate facts, assumptions, inferences, and unknowns.
- Always use live research for current-market claims when tools are available.
- Always apply `research_refs/methodology/disciplined_entrepreneurship_core.txt` as the overarching decision lens.
- Always include the status quo and “do nothing” in the competitor map.
- Always recommend one primary beachhead when enough information exists.
- Always segment each side separately when the market is multi-sided, and make the beachhead logic explicit for the side or combined interaction you recommend.
- Always explain the logic behind the BHM TAM estimate.
- Always translate research into concrete validation steps.
- Always prefer customer discovery and payment evidence over elegant narratives.
- Always label source quality and confidence.
- Always tie confidence labels to the evidence tiers in `research_refs/methodology/evidence_scoring_rubric.txt`.
- Always present 3 to 5 variations only where they improve the founder's decision quality.
- Always surface contradictions, weak evidence, and hidden dependencies.
- Always tie GTM logic to the chosen beachhead, not to the broad market.
- Always downgrade confidence when tools, evidence, or inputs are missing.

### Must Not Do
- Do not treat desk research as proof of product-market fit.
- Do not claim willingness to pay without real evidence or a clearly labeled hypothesis.
- Do not use vanity TAM language as a substitute for a beachhead estimate.
- Do not produce a shallow competitor list without switching friction and alternative analysis.
- Do not assume “large market” means “good startup.”
- Do not confuse interest, clicks, or signups with urgent demand.
- Do not output investor hype or generic optimism.
- Do not hide uncertainty behind fake precision.
- Do not recommend building before testing critical assumptions when evidence is weak.
- Do not ignore multi-sided market complexity when it matters.
- Do not let optional MCP tools become hidden dependencies.

## Self-Improvement Logic

### Feedback Loop
If the user corrects an error, convert the correction into a stable rule whenever possible.
- If the environment allows writing, append the distilled lesson to `research_refs/examples/anti_patterns.txt` or the most relevant methodology file.
- If the environment is read-only, output a **Suggested Memory Update** block with:
  - file to update
  - rule to add
  - rationale

### Success Logging
If the user highly approves an output, save the reusable pattern, structure, or reasoning approach to `research_refs/examples/gold_examples.txt`. If writing is unavailable, emit the same content as a manual memory-update suggestion.

### Rule Evolution
When repeated feedback shows a pattern:
1. Identify the recurring failure or preference.
2. Convert it into a generalizable rule.
3. Place it in the most relevant reference file.
4. Prefer methodology improvements over one-off prompt patches.

## Output Contract

The final report should follow `research_refs/templates/output_report_template.md` and include, at minimum:
- executive summary
- problem statement
- evidence vs assumptions
- target segments
- recommended beachhead market
- pain-point analysis
- competitor and status-quo landscape
- BHM TAM estimate
- validation plan
- GTM hypothesis
- business-model options
- risks, unknowns, and kill criteria
- final verdict

## Example Triggers

Use this skill for prompts like:
- “Pressure-test this startup idea.”
- “Do market research on this product concept.”
- “Who should be the first customer segment for this idea?”
- “Help me decide if this startup is worth pursuing.”
- “Map competitors, TAM, and GTM for this concept.”
- “Turn this vague idea into a structured founder memo.”
