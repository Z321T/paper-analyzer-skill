# Review Standards

Evaluate the claim against the evidence actually available, using the relevant [paper type](paper-types.md). The [Review template](modes/review.md) defines output structure; this file defines judgment criteria.

## What makes a useful review

- A summary identifies the problem, claimed contribution, approach, and central evidence before evaluating them.
- A strength or weakness cites an actual section, table, figure, proof, or identifiable passage.
- A concern explains its consequence for a specific claim and proposes a proportionate way to resolve it.
- Questions are answerable, specific, not already answered in reviewed material, and consequential for the assessment.
- Separate missing evidence, counterevidence, inaccessible material, and inapplicable criteria.

## Criteria

| Dimension | Questions |
| --- | --- |
| Novelty | What do the authors claim is new? How does it differ from identified prior work available at the time? Has this comparison actually been checked? |
| Significance | Which problem or audience benefits, under what assumptions and scale? |
| Correctness | Are definitions, assumptions, derivations, algorithms, and conclusions consistent? |
| Evidence | Do the experiments, proofs, observations, or synthesis support the exact scope of the claims? |
| Comparisons | Are baseline selection and evaluation conditions fair for the relevant historical context? |
| Clarity | Could a reader follow the method/argument and distinguish observations from interpretation? |
| Verification readiness | Are the relevant materials and protocols sufficient to check the key results? |

Check relevant failure modes, rather than applying a universal ML checklist: overgeneralization; data leakage; unmatched baselines; selection bias; omitted assumptions; invalid proof steps; causal claims without causal identification; unjustified metrics; missing uncertainty where it affects the conclusion; component attribution without a suitable test; or unreported details needed to verify a result.

“Not statistically tested” does not establish “no improvement.” “No ablation” matters when a component contribution is claimed; it is not automatically a flaw in a theorem, survey, or teaching note. A small percentage change may matter depending on baseline, uncertainty, and task.

Describe observable gaps. Do not infer dishonesty, deliberate obscurity, or cherry-picking solely from missing information. If a supplement could resolve a concern but is inaccessible, mark the concern provisional.

## Claim–evidence mapping

1. Extract central claims from the abstract/introduction/conclusion, then check their precise qualifications in the body.
2. Locate the relevant experiment, proof, observation, or systematic synthesis.
3. Record the tested/proven scope, assumptions, and alternative explanations.
4. Assess support using the rubric below; justify the label rather than counting experiments.

| Assessment | Meaning |
| --- | --- |
| Strong | Evidence directly establishes the claim within its stated scope; key assumptions and plausible alternatives are addressed. A valid proof can qualify without experiments. |
| Adequate | Evidence supports a bounded conclusion, with limitations that should remain explicit. |
| Weak | Indirect, ambiguous, or insufficient evidence for the stated breadth of the claim. Qualitative evidence is not inherently weak; judge its design and fit. |
| Unsupported in reviewed material | The relevant accessible material contains no adequate backing for the claim. This does not prove the claim false. |
| Contradicted | Identifiable evidence or a valid counterexample conflicts with the claim under its stated assumptions. |
| Unknown | Required material could not be inspected, or interpretation remains unresolved. |

### Synthetic calibration examples

- Claim: “All processing stays on device.” Evidence: inspected architecture specifies no remote processing. This supports the architecture claim to that inspected extent; it does not establish actual runtime behavior unless checked.
- Claim: “The system guarantees complete privacy.” Evidence: only the same local architecture. Support is insufficient for the broader claim without a threat model and relevant analysis; this is not evidence that a leak occurred.
- Claim: “Accuracy improves on split A.” Evidence: the same protocol reports 80% versus 82%. The point estimate increases by 2 percentage points; significance and generalization remain unknown without further evidence.
- Claim: “The identity holds for every positive integer.” Evidence: correct base case and complete inductive step. The proof may strongly support the theorem without code, weights, or experiments.

## Severity and recommendation

A major issue changes the validity or scope of a central conclusion, or blocks checking it. A minor issue affects presentation or a bounded detail without overturning the main result. Explain severity from consequences, not from checklist counts.

Use a supplied venue rubric when the user requests a submission-style recommendation. Without one, prioritize a justified narrative assessment; if the user explicitly asks for accept/reject, state the assumed standard. Do not invent venue-specific numeric scales. Novelty and correctness are separate: a known correct identity may be useful teaching material without being a novel research contribution.

Describe confidence through actual coverage and checks: complete vs excerpted source, inspected proofs/tables/supplements, verified comparisons, and unresolved ambiguities. Do not claim personal expert credentials or certainty based only on fluent exposition.
