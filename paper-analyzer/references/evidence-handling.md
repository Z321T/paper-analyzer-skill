# Source and Evidence Handling

## Reading contract

Identify the title, version/year, and source from available material. Include authors, venue, affiliations, DOI, or project links only when present or verified; mark uncertain publication status rather than guessing. Prefer a short identity line to a wall of missing metadata.

Check the available coverage: abstract, main text, figures/tables, references, appendices, supplements, and optionally code. A short scope note is enough for complete material; prominently disclose missing or unreadable portions when they affect conclusions.

For PDFs, check page coverage and a representative methods/results page for column order, legible formulas, and intact table headers. When extraction is incomplete, use page rendering/vision or OCR if available. If a key item remains unreadable, identify it and restrict the conclusion. Never infer cells from nearby prose or describe unseen figure contents.

Use a nearby translation as assistance only after matching title/version and section structure. Original text and original tables govern factual conflicts. Do not mix results from different versions without labels. If only a translation is available, say so where the distinction affects interpretation.

Read supplied supplementary material when it bears on the question. If a referenced appendix is missing, say “not available in the supplied material,” not “the authors omitted it.” Check an accessible source link when useful; avoid turning a focused reading task into an unrestricted literature search.

For long papers, work through relevant sections in manageable chunks and keep a coverage note. A brief overview may read selectively and disclose this. A section-by-section request requires covering the requested sections in order; if limits prevent completion, identify completed and outstanding sections instead of claiming the whole paper was read. Split long deliverables into clearly named parts/files when appropriate to the user's requested destination, preserving the requested scope, depth, and order.

## Evidence states

| State | Meaning | Example wording |
| --- | --- | --- |
| Reported | Directly stated in accessible paper material | “Table 2 reports…” |
| Verified externally | A source was actually inspected | “Repository documentation checked on [date] states…” |
| Inferred | A deduction or calculation with identifiable premises | “From the stated formula, I infer…” |
| Hypothesized | A plausible explanation or prediction not established by available evidence | “One untested possibility is…” |
| Not reported in reviewed material | Searched the relevant accessible material without finding it | “No seed values were found in the supplied main text; appendix unavailable.” |
| Unknown / unverified | Insufficient access or no check performed | “Code availability not verified.” |
| N/A | Criterion does not apply to this kind of work | “Training seeds: N/A for this deterministic proof.” |

A missing code URL is not evidence that code is closed. A failed request/404 is an access observation, not proof that no repository exists. A paper's promise to release code is a reported promise, not a verified release. Reading repository files does not establish that the experiments execute or reproduce the results.

## Traceable claims and numbers

For each central result or substantive criticism retain: claim, source location, relevant setting, and interpretation. Use a small evidence table for complex analysis; concise inline locations suffice for short answers. For Markdown without page numbers, use its actual headings, equation labels, or a short identifiable passage. Never invent page, table, or section numbers.

Quantitative results should retain the relevant dataset/split, metric and direction, model/setting, baseline, and uncertainty when reported. Write “uncertainty not reported” rather than inventing significance. For an improvement from 80% to 82%, the absolute change is 2 percentage points and the relative increase is 2.5%; explain which quantity is used. Compare losses/latency with their lower-is-better direction intact.

When interpreting an equation, preserve its assumptions, domains, notation, and variable definitions. Label added derivations or numerical examples as your explanation, not an experiment from the paper. Flag unreadable or inconsistent notation instead of silently choosing a convenient replacement.

## External verification

When the user requests background research, actually consult available primary sources or disclose retrieval limits. Bound the search by the question: establish the relevant research context, closest predecessors, and the specific change this paper makes. Do not automatically expand ordinary paper reading into a literature review. Stop when the needed context is supported, or state the unresolved gap. If later developments matter, distinguish them from what was known at publication time.

Use primary sources (paper, official project/repository, proceedings) for bibliographic facts and implementation status. Label the checked version/date for changing facts. Treat citation counts as optional and usually omit them; if requested, report provider and retrieval date.

Distinguish “the authors claim novelty” from an independently checked novelty conclusion. Judge baseline adequacy against relevant work available at the paper's time; discuss later progress separately. Do not fabricate related papers or precise metadata to fill a reading list. If retrieval is unavailable, use only identified references from the accessible paper and disclose the verification limit.
