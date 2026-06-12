# LLM Benchmark Reliability Evidence Cards

## LLMEVAL-2020-F1

Source: Hendrycks et al., 2020. "Measuring Massive Multitask Language Understanding." https://arxiv.org/abs/2009.03300

Finding: MMLU evaluates models across 57 academic and professional subjects using multiple-choice questions.

Author interpretation: The authors present MMLU as a broad test of multitask language understanding, world knowledge, and problem-solving ability.

Method type: benchmark / evaluation dataset

Population / scope: Language models evaluated on academic and professional multiple-choice tasks.

Effect size and uncertainty: Not a single causal effect; benchmark accuracy is the reported measure.

Direction of support:

| Theory | Direction | Note |
| --- | --- | --- |
| T1 Broad Capability Signal | supports | Supports the idea that benchmark breadth can reveal broad capability differences. |
| T2 Narrow Construct Signal | scope-limits | Multiple-choice academic coverage may not capture all forms of capability. |

Strength grade: 2

Conflicts with: none known

Funding / incentive note: Academic research paper.

Status: active

## LLMEVAL-2022-F1

Source: Liang et al., 2022. "Holistic Evaluation of Language Models." https://arxiv.org/abs/2211.09110

Finding: HELM evaluates models across multiple scenarios and metrics, including accuracy, calibration, robustness, fairness, bias, toxicity, and efficiency when possible.

Author interpretation: The authors argue that language-model evaluation should be broader and more transparent than single-metric task accuracy.

Method type: benchmark / evaluation framework

Population / scope: Thirty language models across selected scenarios and metrics in the HELM release.

Effect size and uncertainty: Multiple reported metrics; no single summary effect.

Direction of support:

| Theory | Direction | Note |
| --- | --- | --- |
| T3 Multi-Metric Evaluation | supports | Supports the claim that benchmark interpretation requires multiple desiderata. |
| T1 Broad Capability Signal | scope-limits | A single accuracy score cannot carry every evaluation claim. |

Strength grade: 3

Conflicts with: none known

Funding / incentive note: Academic research project with public release of prompts and completions.

Status: active

## LLMEVAL-2022-F2

Source: Srivastava et al., 2022. "Beyond the Imitation Game: Quantifying and extrapolating the capabilities of language models." https://arxiv.org/abs/2206.04615

Finding: BIG-bench contains 204 tasks contributed by a broad group of authors, with findings that performance patterns vary by task and scale.

Author interpretation: The authors present BIG-bench as a way to study diverse capabilities and limitations that may not be captured by narrower benchmarks.

Method type: benchmark / evaluation dataset

Population / scope: Language models evaluated across a large task collection.

Effect size and uncertainty: Task-specific performance; no single effect size.

Direction of support:

| Theory | Direction | Note |
| --- | --- | --- |
| T1 Broad Capability Signal | supports | Broad task collections can reveal cross-task patterns. |
| T2 Narrow Construct Signal | scope-limits | Task-level variation warns against overgeneralizing from one score. |
| T3 Multi-Metric Evaluation | supports | Diverse tasks expose multiple dimensions of performance. |

Strength grade: 3

Conflicts with: none known

Funding / incentive note: Large collaborative research project.

Status: active

## LLMEVAL-2023-F1

Source: Li, Guerin, and Lin, 2023. "An Open Source Data Contamination Report for Large Language Models." https://arxiv.org/abs/2310.17589

Finding: The authors report varying contamination levels across models and benchmarks, and find that contamination does not always translate into a large metric gain.

Author interpretation: The authors argue that contamination analysis is an important part of reliable model evaluation and should be more transparent.

Method type: contamination analysis

Population / scope: Popular language models and multiple-choice QA benchmarks included in the study.

Effect size and uncertainty: Reported contamination levels vary by model and benchmark; relationship to score gains varies.

Direction of support:

| Theory | Direction | Note |
| --- | --- | --- |
| T2 Narrow Construct Signal | supports | Benchmark scores can be shaped by benchmark familiarity or overlap. |
| T3 Multi-Metric Evaluation | supports | Supports adding contamination checks before interpreting scores broadly. |
| T1 Broad Capability Signal | undercuts | Undercuts simple score-to-capability interpretation when contamination is plausible. |

Strength grade: 3

Conflicts with: LLMEVAL-2020-F1 as a scope conflict, not a direct contradiction

Funding / incentive note: Academic research paper.

Status: active

## LLMEVAL-2023-F2

Source: Deng et al., 2023. "Investigating Data Contamination in Modern Benchmarks for Large Language Models." https://arxiv.org/abs/2311.09783

Finding: The authors propose methods for detecting benchmark contamination and report evidence that some models can guess missing benchmark test data elements.

Author interpretation: The authors argue that benchmark contamination creates concerns for robust evaluation, especially when training data transparency is limited.

Method type: contamination analysis

Population / scope: Open-source and proprietary language models evaluated against selected benchmarks.

Effect size and uncertainty: Reported exact-match rates and contamination indicators vary by benchmark and method.

Direction of support:

| Theory | Direction | Note |
| --- | --- | --- |
| T2 Narrow Construct Signal | supports | Supports concern that some scores may reflect benchmark exposure. |
| T3 Multi-Metric Evaluation | supports | Supports using contamination checks as part of evaluation. |
| T1 Broad Capability Signal | undercuts | Undercuts broad interpretation when test data exposure is plausible. |

Strength grade: 3

Conflicts with: LLMEVAL-2020-F1 as a scope conflict, not a direct contradiction

Funding / incentive note: Academic research paper.

Status: active

