# Reading / 阅读

Help the reader understand the paper well enough to explain its mechanism and the reach of its evidence. Follow the routing and presentation rules in [SKILL.md](../../SKILL.md).

## Fit the explanation to the request

- Default to substantive explanation organized around the research logic below. Allocate space to the few concepts that determine understanding; do not give every section equal length or mechanically print every heading.
- For a quick overview, concentrate on the problem, key mechanism, central result with conditions, and the most consequential boundary. Honor the requested length or time budget; a short answer can still explain a difficult idea precisely.
- For section-by-section or paragraph-by-paragraph requests, preserve the original order, numbering, and recognizable headings. Cover every requested section and relevant accessible appendix, including less central ones. Explain claims, equations, and visible figures in place. If completion requires multiple parts, identify completed and outstanding coverage; do not silently replace the request with a thematic summary.
- For faithful exposition, keep the authors' account distinct from added explanatory examples and deductions; omit evaluative overlays when the user excludes them.
- For a focused follow-up, answer the local question using already-read material. Supply only the surrounding context needed to understand it.

## Develop the research logic

Begin a complete reading with the paper's identity, a one-sentence takeaway, and any material coverage limits. Adapt the following sequence to the paper type and the user's requested order.

**Problem and value.** Specify what is given, what must be achieved, and the constraints that make it difficult. Explain who benefits and what concrete capability or cost could change; distinguish demonstrated value from anticipated applications.

**Relevant prior approaches and bottleneck.** Explain the most directly relevant predecessor or alternative, what it already solves, and the remaining limitation under comparable assumptions. Do not imply that an entire problem was unsolved merely because this paper improves one setting. Background research follows the scope and verification guidance in [evidence-handling.md](../evidence-handling.md).

**Core observation and intuition.** State the key observation in plain language, then explain how it motivates the proposed design. Distinguish the authors' motivation from your explanatory reconstruction. An analogy may introduce the idea, but connect it back to the actual objects and operations. A plausible intuition is not evidence of effectiveness.

**Method or argument.** Explain how each consequential operation changes its input and why it is needed. When helpful, use the same concrete example from input through intermediate states to output. Read the relevant [explanation guidance](../explanation-guidance.md) for worked examples and equations. For theory, trace assumptions, lemmas, and the decisive proof step; for a survey or qualitative study, explain the taxonomy or analysis procedure instead of forcing a computational pipeline. Keep training and inference distinct when applicable.

**Evidence and interpretation.** Explain what experiment, proof, observation, or synthesis supports each central claim. Preserve settings, metric direction, source locations, and reported uncertainty. A result table is useful when comparison benefits from it, not a compulsory section. Discuss component attribution, fair baselines, or generalization when they affect the interpretation. A claim that a component is necessary needs appropriate evidence or an explicit hypothesis label.

**Contribution and boundary.** Connect the supported advance to the original problem. Explain decisive assumptions, failure cases, and what remains unresolved. Separate observed failures from plausible concerns. Avoid unsupported impact ratings or fixed reading-list quotas.

## Add depth only where it serves the task

- Embed critical checks beside the mechanism or result they concern. A reviewer's perspective need not produce a referee report. Use [review-standards.md](../review-standards.md) when judging claim validity.
- Ordinarily mention only implementation or verification conditions that matter to understanding the result. Load [reproducibility-checklist.md](../reproducibility-checklist.md) and expand a readiness assessment when requested or when a material obstacle warrants it; do not automatically append a full status table.
- Select visuals using [visualization-guidance.md](../visualization-guidance.md), place them with the concept they explain, and discuss what the reader should notice.
- For a paper discussion, add a useful narrative, source figures, likely questions, and timing when supplied. A request to understand a paper is not a request to create slides.

Finish with the most useful supported interpretation or open question. Do not append a mandatory question, checklist, or redundant summary.
