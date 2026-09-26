# Adapt Criteria to the Paper

Classify the contribution before applying a template. Mixed papers can use multiple rows. This is a choice of relevant checks, not a reason to invent missing sections.

| Paper type | Main evidence to examine | Reproduction / verification materials | Usually inapplicable |
| --- | --- | --- | --- |
| Empirical ML / statistical methods | Task definition, datasets/splits, baselines, uncertainty, component tests where causal claims need them | Data, preprocessing, model/configuration, training or inference procedure, evaluation protocol | Training/weights for training-free methods |
| Theory / mathematical proof | Definitions, assumptions, theorem scope, proof steps, counterexamples, relation to known results | Complete derivations/proofs and computational tools if used | Datasets, training seeds, weights, empirical ablations for purely analytic work |
| Survey / systematic review | Search scope/date, inclusion/exclusion, coverage, taxonomy, synthesis and selection bias | Search queries, screening/extraction protocol, source corpus when applicable | Model training and module ablations; systematic-review criteria for an explicitly narrative survey |
| Dataset / benchmark | Collection, provenance, annotation quality, splits/leakage, metric validity, licensing/access | Dataset/version, documentation, annotation protocol, evaluation scripts | Model novelty; training details if no model is trained |
| Systems / algorithms | Correctness, complexity, workloads, hardware/software, performance tradeoffs, comparison fairness | Implementation, environment/configuration, workloads, run commands | Learned weights, optimizer settings and random seeds for deterministic non-learning methods |
| Qualitative / observational study | Sampling, data collection, coding/analysis, triangulation, reflexivity, causal limits | Study/analysis protocol and access constraints; protected data need not be public | Training, model weights, ML ablations; blanket statistical-significance requirements |

Within the chosen type, tailor the output:

- In Reading → Deep, replace “training details” with “proof assumptions,” “review protocol,” or “implementation details” when appropriate. Replace method pipelines with argument structure or omit redundant diagrams.
- In Review, evidence can be a proof, observation, qualitative analysis, or an experiment. An absence of experiments does not by itself imply an unsupported theorem or qualitative finding.
- In reproduction readiness, identify which materials are necessary for the key claim. A teaching note can be correct and verifiable without being novel. A privacy-restricted dataset can present a real access barrier without implying poor scientific conduct.
- Use N/A with a reason for irrelevant criteria. Use unknown for unseen material. Do not count either as a failed requirement, and do not average them into a numeric score.
