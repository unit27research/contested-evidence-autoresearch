# LLM Benchmark Reliability Question Backlog

## RQ-LLMEVAL-001

Generated from: AUTOPSY-LLMEVAL-001

Question:

How much does benchmark exposure change the interpretation of a score for a specific model family and benchmark?

Theories discriminated:

- T1 Broad Capability Signal
- T2 Narrow Construct Signal
- T3 Multi-Metric Evaluation

Pre-commitment:

If performance stays similar across public, contamination-screened, and fresh held-out items testing the same construct, confidence in T1 goes up. If performance drops materially on fresh or contamination-screened items, confidence in T2 and T3 goes up.

Prioritization:

| Axis | Score | Note |
| --- | ---: | --- |
| Discrimination power | 3 | Directly tests broad score interpretation. |
| Feasibility | 2 | Requires item construction or access to contamination-screened sets. |
| Confidence leverage | 3 | Would move the strongest undercut against T1. |

Status: backlog

## RQ-LLMEVAL-002

Generated from: T2 empty undercutting section

Question:

When does a benchmark score generalize well enough to support a broader capability claim?

Theories discriminated:

- T1 Broad Capability Signal
- T2 Narrow Construct Signal

Pre-commitment:

If benchmark score predicts performance on independently constructed tasks with changed format and distribution, confidence in T1 goes up. If the relationship breaks under modest format or distribution shifts, confidence in T2 goes up.

Prioritization:

| Axis | Score | Note |
| --- | ---: | --- |
| Discrimination power | 3 | Separates broad capability from narrow construct performance. |
| Feasibility | 2 | Requires paired benchmark and held-out task data. |
| Confidence leverage | 3 | Clarifies what claim the benchmark can support. |

Status: backlog

## RQ-LLMEVAL-003

Generated from: T3 distinctive prediction

Question:

Do models with similar benchmark accuracy differ materially on calibration, robustness, fairness, efficiency, or contamination risk?

Theories discriminated:

- T1 Broad Capability Signal
- T3 Multi-Metric Evaluation

Pre-commitment:

If models with similar accuracy show materially different profiles on other metrics, confidence in T3 goes up. If accuracy predicts the relevant downstream metrics well enough for the decision at hand, confidence in T1's practical usefulness goes up for that setting.

Prioritization:

| Axis | Score | Note |
| --- | ---: | --- |
| Discrimination power | 2 | Strong for evaluation design, less direct for benchmark validity. |
| Feasibility | 3 | HELM-style multi-metric data can support this analysis. |
| Confidence leverage | 2 | Clarifies when single-score reporting is insufficient. |

Status: backlog

