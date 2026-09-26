# Reading / 阅读

Choose one reading type using [SKILL.md](../../SKILL.md), then consult only its section: [Skim / 速读](#skim), [Walkthrough / 详解](#walkthrough), or [Deep / 精读](#deep). These are alternatives within Reading, not three outputs to generate together. User scope and format remain controlling.

## Skim

Deliver a short decision aid: what the paper does and whether a deeper read is useful. Use the length and diagram defaults in [SKILL.md](../../SKILL.md), unless the user specifies otherwise.

1. **Identity and takeaway**: title, known authors/year if useful; one sentence on the problem, approach, and supported result.
2. **Core problem**: why it matters and the limitation being addressed, in 1–2 sentences.
3. **Method**: the main mechanism or argument, in 2–3 sentences. A diagram is optional; do not draw one merely to fill a slot.
4. **Key evidence**: 1–3 central findings with source locations and essential conditions. If only the abstract is available, attribute these to the abstract. For theory, use the theorem and assumptions rather than demanding benchmark numbers.
5. **Reading value and caveat**: who benefits, and one important limitation or unanswered question when supported.

Omit absent nonessential metadata. If code status is requested but not checked, say “unverified.” Avoid full review tables, compulsory ratings, and follow-up boilerplate.

## Walkthrough

Provide a faithful reading companion in the original section order. Explain what the authors say without adding a review or novelty score. Correcting a translation/extraction error or explaining an ambiguity is compatible with faithful exposition.

### Structure

Start with identity, takeaway, and material coverage. Include a table of contents for a long output when useful.

For each requested section and subsection, preserve the original numbering and make the source heading recognizable in the output language:

- **Original points**: the claims, definitions, reasoning, and findings stated by the authors.
- **Technical explanation**: important formulas with variables and assumptions; step-by-step reasoning where needed. Clearly label any derivation or example you add as an explanation.
- **Figures and tables**: describe accessible content, relevant conditions, and what the authors use it to demonstrate. If only a caption is visible, identify that limit instead of reconstructing the image.
- **Section synthesis**: briefly connect the section to the paper's argument, at major section boundaries only.

Cover accessible appendices relevant to the requested walkthrough in their actual order/labels. A missing supplement is a coverage limit, not grounds to invent appendix content.

### Presentation adaptation

If preparing a paper discussion, optionally finish with a narrative, recommended source figures, time allocation if a duration is known, and likely questions grounded in the text.

Keep evaluative criticism, innovation ratings, and reproduction judgments for a requested analytical component. Diagram policy follows the [entrypoint](../../SKILL.md); an explicitly requested explanatory diagram must remain faithful to the source.

## Deep

Analyze how the paper works and how far its evidence supports its contribution. Adapt section content using [paper-types.md](../paper-types.md); user scope and available material determine the depth.

Start with identity, a one-sentence takeaway, and coverage. Provide an overview mindmap and method/argument diagram when they improve understanding under the [entrypoint's diagram policy](../../SKILL.md). Place each diagram with the relevant discussion.

### 1. Problem and motivation

Explain the task, assumptions, why it matters, and the specific limitation the authors address. Separate the authors' framing from an independently verified comparison to prior work.

### 2. Method or argument

Explain the overall structure, then each important component:

- Design motivation or logical purpose.
- Mechanism, equations, assumptions, and information flow.
- Difference from identified prior approaches when supported.
- Known constraints and your explicitly labeled possible concerns.

Include training/inference configuration for applicable ML work, proof dependencies for theory, or protocol/implementation details for other types. Label added derivations as explanations. Do not fill unseen technical details from generic domain expectations.

### 3. Evidence and results

Describe experiments, proofs, observations, or synthesis appropriate to the paper. For quantitative work, give a compact results table retaining metric direction, conditions, source locations, and reported uncertainty. Examine fair comparisons, relevant component tests, robustness, and limits of generalization. Distinguish missing evidence from evidence against a claim.

### 4. Contribution and limits

Describe each claimed contribution, the support for it, and its scope. Identify conceptual, methodological, empirical, or engineering contributions where useful. Avoid ungrounded High/Medium/Low impact ratings. Counterfactual statements such as “without this component…” require an ablation/proof or an explicit hypothesis label.

### 5. Related work and implications

Use identifiable references from the paper or actually checked primary sources. Explain meaningful differences; no fixed quota of “must-read” papers. Separate speculative future directions from established findings. For excerpts without references, omit the reading list or state the limit.

### 6. Reproduction or verification readiness

Read [reproducibility-checklist.md](../reproducibility-checklist.md). Include an applicable status table and key obstacles; unknown and N/A are distinct from failure. State whether the assessment is based on documentation or actual execution. If the user excludes tables, express the same relevant conclusions in the requested format.

### 7. Discussion / paper presentation

Finish with the most consequential interpretation or open question supported by the analysis. If preparing a presentation, suggest a narrative, source figures, and anticipated questions; tailor timing to a supplied duration. Do not require a follow-up question.
