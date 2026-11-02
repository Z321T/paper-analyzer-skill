# Budgeted Candidate Routing (synthetic teaching paper)

This is invented test material, not a publication. No external bibliographic or novelty claims are supplied.

## 1. Problem

Rank a finite candidate set for a query using at most k expensive score evaluations. Cheap scores are available for all candidates. The motivating constraint is expensive scorer calls, not measured wall-clock latency.

## 2. Method

For each candidate i, compute a cheap score a_i. Select the k candidates with largest a_i. Evaluate an expensive score b_i only for those candidates, then return the selected candidate with largest b_i. Ties use ascending candidate ID. Here i indexes candidates and k is an integer between 1 and candidate count. Training, score computation internals, and code location are not supplied.

## 3. Worked example

For query Q, candidates A, B, C have cheap scores 0.9, 0.8, 0.1. Set k=2. Expensive scores for A and B are 0.4 and 0.7; return B. C's expensive score is not evaluated. No ground-truth relevance label is supplied.

## 4. Results

Table 1, synthetic split S with 100 queries: k=2 routing reports accuracy 82%; evaluating all candidates reports 80%. The average candidate count is 10. No uncertainty, repeated runs, or latency measurements are supplied. The authors describe routing as using fewer expensive scorer calls in this setting; the result does not establish general superiority.

## Appendix A. Limitation

A candidate excluded by cheap scoring cannot be recovered by expensive reranking. Smaller k may therefore discard the best expensive-scoring candidate. No monotonic accuracy guarantee is given.
