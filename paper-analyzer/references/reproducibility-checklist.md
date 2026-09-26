# Reproduction and Verification Readiness

Assess whether someone could independently check the paper's key result with the documented materials. This is a readiness assessment, not a claim that reproduction has been performed. Readiness and scientific evidence strength are separate judgments.

Use the applicable [paper-type criteria](paper-types.md). Review accessible supplements before declaring information absent. Code, weights, training, and public datasets are not universal requirements.

## Status vocabulary

| Status | Meaning |
| --- | --- |
| ✅ Sufficient | The relevant inspected materials adequately specify this dimension. Say what was inspected. |
| ⚠️ Partial | Inspected materials provide some needed information but leave a concrete gap. |
| ❌ Missing / obstructed | A required item is confirmed absent from the reviewed material or blocked under the stated conditions. Name that scope; do not imply universal unavailability. |
| ? Unknown / unverified | Not inspected, inaccessible, or insufficient information to determine status. |
| N/A | Not needed for this paper's central result. Give a brief reason. |

Missing a link in the paper means external code status is unknown, not necessarily closed. A statement of intended release is not a verified release. Restricted data may require an access process; assess that process and the resulting barrier rather than equating restricted licensing with invalid science.

## Dimensions to select

| Dimension | Relevant checks |
| --- | --- |
| Code / computational artifacts | Official location and inspected version; implementation needed for the claim; dependencies and commands; configurations; weights only if the method needs them; actual license/access conditions. Distinguish author-reported availability from inspected contents and from successful execution. |
| Data / study material | Identity/version, access or documented acquisition process, generation/collection protocol, preprocessing, splits, annotation, provenance, and permitted use. For protected data, record accessible protocols and unresolved barriers. |
| Method / protocol / proof | Definitions and assumptions; complete derivation or procedure; for ML, applicable architecture, optimizer, schedule, batch/steps, seed policy, prompts, hardware; for reviews/studies, search/sampling/analysis protocol. |
| Evaluation procedure | Metric formulas/aggregation, test conditions, evaluation code or proof-checking route, randomization and uncertainty where relevant, human/LLM evaluation procedure when used. |
| Resources and environment | Software/hardware versions and compute needs when material to reproduction. For manual proof verification this may be N/A. |

For a purely analytic paper, prioritize proof completeness and assumptions and mark computational dimensions N/A. For inference-only work, training details may be N/A while model version, prompts, decoding, and evaluation remain essential. For a review, replace model/data checks with search, screening, extraction, and synthesis materials as appropriate.

## Report

Use a compact table in Reading → Deep and Review unless the user's format excludes tables. Select meaningful rows; do not add irrelevant rows merely to fill a fixed five-part score.

| Applicable dimension | Status | Evidence / location / inspected scope | Remaining obstacle |
| --- | --- | --- | --- |

Then state:

- **Basis**: paper/excerpt/supplement/repository inspected; whether anything was actually run.
- **Readiness**: high, medium, low, or undetermined, with the decisive reason.
- **Next check**: the concrete material or check needed to resolve the most important uncertainty, if any.

| Readiness | Meaning |
| --- | --- |
| High | Relevant accessible materials are sufficient to verify key results; this remains a documentation-based assessment unless execution was performed. |
| Medium | A plausible route exists, with specific gaps or substantial effort. |
| Low | Confirmed material/access barriers prevent checking important results under the stated conditions. |
| Undetermined | Too much necessary material is uninspected or unavailable to make an overall judgment, as with an abstract alone. |

Do not average statuses, count N/A as failure, or convert unknown into low readiness. A known decisive obstacle may justify low readiness despite other unknowns, but name that obstacle precisely. Reserve claims of failed reproduction for an actual attempt with recorded conditions and discrepancies; lack of documentation alone does not prove a result impossible to reproduce.

## Evidence quality is a separate question

Ablations, matched baselines, robustness tests, and uncertainty address how convincingly the claims are supported. Discuss them in the evidence/review section. Their absence can weaken a causal or performance claim even when the available experiment is easy to rerun. Conversely, persuasive reported results may remain hard to reproduce because required artifacts are inaccessible.

## Optional resource estimate

Estimate compute only when useful and inputs are supplied or verified. Show assumptions and arithmetic: device count × hours × runs. Distinguish training, tuning, and evaluation. For money estimates, include the actual price source/date and currency, or explicitly use a hypothetical rate; do not present an old example price as current. Avoid asserting affordability for an unspecified lab or user.
