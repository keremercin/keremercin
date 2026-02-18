# How I Evaluate RAG Systems Under Budget Constraints ($0-30)

## Why this matters
Most RAG projects optimize prompt quality, but skip evaluation discipline. Without quality gates, improvements are anecdotal.

## Principles
1. Keep evaluation deterministic first, model-judge second.
2. Track retrieval and answer quality separately.
3. Group failures into actionable buckets.
4. Keep costs low by using small synthetic/public scenarios before scaling.

## Minimal metric set
- `precision@k`
- `recall@k`
- `mrr`
- answer relevance heuristic

## Failure buckets
- `hallucination`
- `missed_citation`
- `stale_context`
- `ok`

## Practical workflow
1. Run benchmark scenarios (legal + support).
2. Compare metrics to baseline from previous release.
3. Inspect changed failure buckets.
4. Only ship if regression thresholds pass.

## Repo reference
Implementation: [rag-eval-observatory](https://github.com/keremercin/rag-eval-observatory)
