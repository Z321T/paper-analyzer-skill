# Visual Explanations

Choose a visual to answer a specific question, not to meet a quota. Follow user preferences and available host capabilities. Place the visual beside the relevant explanation and state what its structure or variation reveals.

## Choose the representation

| Understanding obstacle | Useful representation |
| --- | --- |
| What happens in which order; what information moves between steps? | Flowchart, state transition, or annotated running example |
| How does a parameter affect a stated mathematical quantity? | Curve with labeled axes, domain, and fixed assumptions |
| How do observations vary or relate? | Distribution or scatter plot using accessible data |
| What does the operation mean geometrically? | Coordinate diagram or projection with defined objects |
| What changes when an input or parameter is varied? | Interactive view when supported and more informative than a static figure |
| How do methods compare under stated conditions? | Aligned table; plot only when quantities are comparable |

Use [Mermaid templates](mermaid-templates.md) only for suitable structural diagrams. A flowchart does not substitute for a requested curve or geometric explanation. Avoid ASCII or text-layout pseudo-charts when a genuine visual is requested.

## Establish provenance before drawing

- **Source figure/table:** identify the paper location and preserve axes, units, conditions, and uncertainty. A caption alone does not reveal the figure contents.
- **Formula-derived figure:** state the source equation, assumed parameter values, range, and what remains fixed. Label it as a mathematical illustration, not an experiment.
- **Teaching schematic:** label constructed numbers and simplifying assumptions. Geometry, arrows, and apparent precision must not imply unreported evidence.
- **Executed result:** report actual input, procedure, environment where relevant, and the scope of what ran. Do not imply reproduction of the paper from a toy calculation.

Do not manufacture samples, benchmark curves, uncertainty bands, or measured accuracy/latency to complete a visual. A few reported points do not justify a smooth empirical curve without a clearly labeled interpolation and its limitations. A monotonic cost formula does not imply monotonic accuracy.

## Deliver with the host's available capabilities

Prefer supported inline figures; use interaction when it helps explore a mechanism. Use standard plotting tools for quantitative or exportable figures and Mermaid for appropriate structure. Do not depend on a particular vendor's visualization API or install a new runtime merely to satisfy a default preference.

If interaction is unavailable, provide a useful static figure when possible and state the difference. If rendering is unavailable, disclose the limitation and provide the supported alternative; do not claim that code or a text description is a rendered chart. An explicitly requested visual that cannot be delivered remains an unmet part of the request.

Check the actual artifact when tools permit: labels, units, scales, legends, numeric agreement, clipping, and agreement with the source. Test interactive parameter changes when present. Disclose unverified rendering or interaction rather than claiming it passed.
