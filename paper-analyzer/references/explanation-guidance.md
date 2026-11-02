# Explaining Mechanisms, Examples, and Equations

Consult the section needed for the current difficulty. The goal is transferable understanding, not a longer answer or imitation of a named researcher.

## Mechanism before terminology

Begin with the concrete obstacle, introduce the key observation, and show how the operation addresses that obstacle. Connect module names to what they actually do. Explain design tradeoffs only to the extent supported by the source; do not invent the authors' intentions.

Infer prerequisite knowledge from the conversation. Define unfamiliar concepts when they first become necessary; skip textbook detours that do not help explain this paper. Use connected prose with concrete claims. Remove boilerplate praise, repeated contrasts, and punctuation that substitutes for an explanation.

## A running example

Prefer a sufficiently detailed example in the paper. Otherwise construct a small teaching example and label its chosen inputs, simplified assumptions, and computed outputs. Never call illustrative numbers, hypothetical model outputs, or invented intermediate states reported results.

Track the same instance through the consequential steps: input object and relevant shape; operation; intermediate representation or candidate set; output and its meaning. Explain what information is retained, discarded, or introduced. If a necessary operation is unspecified, mark the gap and stop the numerical trace there rather than inventing implementation details. A symbolic trace can remain useful.

For a proof, a small case or counterexample can expose the key assumption, but does not replace a general argument. An example is optional when the original explanation is already clear.

### Example of useful specificity

Teaching example, not a paper result: a two-stage ranker keeps two candidates using cheap scores. A, B, C score 0.9, 0.8, 0.1, so A and B survive. Their expensive scores are 0.4 and 0.7, so the final output is B. C's expensive score remains unknown. The expensive stage can change the ordering of survivors, but cannot recover a discarded candidate. This explains the mechanism without claiming the output is correct or the method improves accuracy.

## Equations with meaning

Preserve source notation and assumptions. At first use, define every symbol needed to read the equation, including indices, superscripts, operators, domains, and relevant scalar/vector/matrix shapes. Explain whether a superscript denotes a power, time step, layer, or label. Reuse definitions instead of repeating them for every formula; identify changes of notation explicitly.

Explain the mathematical action in words: what is combined, normalized, compared, or optimized, and how this relates to the method. Show a key derivation step or simple substitution when it resolves a real difficulty. For parameter effects, explain what is held fixed and check boundary cases when informative. Distinguish an exact identity, an approximation, and a heuristic.

Clearly label added derivations and illustrative calculations. A mathematical property of a simplified model is not an observed property of the full system. For unreadable notation, follow [evidence-handling.md](evidence-handling.md) rather than silently repairing it.
