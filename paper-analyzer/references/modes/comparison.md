# Comparison

Compare any two or more papers along dimensions relevant to the user's question. For a large set, group papers or use a compact matrix; do not stop at three or silently omit a paper.

## 1. Scope and identities

Identify each paper/version and available material. State the shared question. Match unlike contributions thoughtfully: a benchmark paper and a method paper may serve different purposes.

## 2. Aligned matrix

Use applicable rows: problem, assumptions, mechanism, model/implementation, data, evidence, compute, access status, strengths, and limits. Attach locations to central numbers or conclusions. Unknown cells remain unknown.

## 3. Comparability check

Before interpreting numerical differences, check:

- Dataset identity/version and train/validation/test split.
- Metric definition, units, aggregation, and higher/lower-is-better direction.
- Model scale, training/pretraining data, supervision, and compute budget.
- Evaluation protocol, prompting (zero/few-shot), retrieval/tools, and uncertainty.
- Hardware, batch size, precision, and workload for speed/cost claims.

Label result pairs **directly comparable**, **indicative only**, or **not directly comparable**, with a reason. Different metric names or splits cannot be ranked by their raw magnitudes. Asymptotic complexity is not measured runtime; smaller model size alone does not establish latency or cost superiority.

## 4. Synthesis and conditional advice

Explain whether approaches are complementary, sequential, or competing using evidence. Add a relationship diagram only when useful and consistent with user preferences. Recommend based on the user's constraints; if these are unknown, present conditional tradeoffs and the measurements needed to choose. Never force a winner from incompatible results.
