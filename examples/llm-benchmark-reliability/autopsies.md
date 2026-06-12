# LLM Benchmark Reliability Autopsies

## AUTOPSY-LLMEVAL-001

Conflicting cards:

- LLMEVAL-2020-F1
- LLMEVAL-2023-F1
- LLMEVAL-2023-F2

Apparent conflict:

MMLU presents a broad multitask benchmark intended to evaluate language-model understanding across many subjects. Later contamination studies argue that benchmark exposure and test-set overlap can make benchmark interpretation less reliable.

Taxonomy:

| Category | Fits? | Reasoning |
| --- | --- | --- |
| A. Different constructs | partial | Benchmark breadth and contamination risk measure different properties. |
| B. Different populations or conditions | yes | The original benchmark claim depends on evaluation conditions; contamination studies examine later model and data conditions. |
| C. Different time periods | yes | Public benchmark exposure changes after release. |
| D. Methodological artifact | partial | Contamination detection methods have their own assumptions. |
| E. Analytic flexibility | partial | Different contamination definitions and detection methods can change interpretation. |
| F. Likely spurious result | no | The cards can coexist. |
| G. Genuine unresolved conflict | partial | The unresolved question is how much contamination changes a specific score interpretation. |

Assigned category:

B and C, with remaining G.

Reasoning:

The cards do not simply contradict each other. A benchmark can be well designed for its original purpose and still become harder to interpret after broad public exposure. The unresolved conflict is not "benchmark valid or invalid." It is when a score supports a broad capability claim versus a narrower benchmark-performance claim.

What would resolve this:

For a given benchmark and model family, compare performance on public items, contamination-screened items, and newly constructed held-out items testing the same claimed construct.

Question generated:

See RQ-LLMEVAL-001.

