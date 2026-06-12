# LLM Benchmark Reliability Theory Map

## T1 Broad Capability Signal

Claim: A high benchmark score can support a broad claim about model capability when the benchmark covers many tasks and the evaluation conditions are trustworthy.

Mechanism:

1. A benchmark samples many relevant tasks.
2. Model performance differs across those tasks.
3. Aggregate performance reflects a real capability difference.
4. The score supports a broad, though still bounded, capability claim.

Distinctive prediction:

Models that score higher should also perform better on related held-out tasks that test the same claimed capability.

Supporting cards:

- LLMEVAL-2020-F1
- LLMEVAL-2022-F2

Undercutting cards:

- LLMEVAL-2023-F1
- LLMEVAL-2023-F2

Scope conditions:

- Benchmark exposure must be low or accounted for.
- The claim should match the benchmark construct.
- A single score should not carry claims about safety, robustness, fairness, or deployment readiness.

## T2 Narrow Construct Signal

Claim: Many benchmark scores support only a narrower claim about performance on a task family, format, or dataset, not a broad capability claim.

Mechanism:

1. A benchmark operationalizes one construct through specific tasks and formats.
2. Models can improve on that operationalization.
3. The score is treated as evidence for a broader capability.
4. The broader claim outruns the measured construct.

Distinctive prediction:

Models with strong benchmark scores may fail on related tasks that change the format, distribution, language, or evaluation setting.

Supporting cards:

- LLMEVAL-2020-F1 as a scope-limited benchmark design card
- LLMEVAL-2022-F2
- LLMEVAL-2023-F1
- LLMEVAL-2023-F2

Undercutting cards:

- none filed; needs a held-out generalization card

Scope conditions:

- The theory is strongest when the public claim is broader than the benchmark task.
- It does not imply benchmarks are useless.

## T3 Multi-Metric Evaluation

Claim: Benchmark scores are useful only when interpreted as part of a multi-metric evaluation that includes calibration, robustness, fairness, contamination, efficiency, and task coverage.

Mechanism:

1. Model quality is multidimensional.
2. Single-task or single-metric scores hide tradeoffs.
3. Multi-metric evaluation makes those tradeoffs visible.
4. Claims become narrower and more inspectable.

Distinctive prediction:

Two models with similar accuracy scores may differ materially on calibration, robustness, fairness, efficiency, or contamination risk.

Supporting cards:

- LLMEVAL-2022-F1
- LLMEVAL-2022-F2
- LLMEVAL-2023-F1
- LLMEVAL-2023-F2

Undercutting cards:

- none filed; needs an example where a single score robustly predicts the downstream decision-relevant outcome.

Scope conditions:

- Multi-metric evaluation can be expensive.
- More metrics do not automatically settle which tradeoff matters.

