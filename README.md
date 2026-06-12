# Contested Evidence Autoresearch

A field kit for using iterative research loops in domains where the evidence is unresolved, the theories compete, and there is no clean scoreboard to optimize against.

Most autoresearch work is strongest when the loop has a measurable target: a benchmark, simulation, executable experiment, loss curve, or pass/fail test. Many real research and policy domains do not look like that. The evidence is mixed. Sources disagree. Terms drift. The strongest available result may depend on scope, population, method, or time period.

This repo proposes a different loop for those settings. The goal is not to force convergence. The goal is to improve the structure of disagreement, preserve uncertainty where it is earned, and produce better next questions.

## Who This Is For

This field kit is for people who need to reason across mixed evidence without pretending the field is cleaner than it is:

- research teams comparing competing causal theories
- policy analysts working with uneven evidence
- investigative researchers building source-backed claim maps
- grant, review, or strategy teams trying to name what is actually known
- organizational teams deciding what evidence to collect next before committing to a position

It is most useful when the team has enough source material to disagree responsibly, but not enough clarity to declare a winner.

## When Not To Use This

Do not use this kit when a cleaner method fits the problem better.

- If there is a clear executable test, run the test.
- If the domain has a validated benchmark or simulation, use it directly.
- If a formal systematic review is required, follow the relevant review protocol and reporting standard.
- If the decision is safety-critical, clinical, legal, or time-sensitive, use qualified domain governance.
- If the team cannot inspect the underlying sources, do not use this framework to create authority from summaries.

This kit is for structured reasoning under uncertainty. It is not a substitute for stronger evidence, formal review methods, or accountable decision-making.

## Core Thesis

In contested fields, a useful research loop should not optimize toward the most confident answer. It should optimize for:

- clearer claim-evidence binding
- better separation between findings and interpretations
- visible conflicts between credible sources
- explicit scope conditions
- adversarial review against the current leading theory
- ranked research questions that would actually move confidence

The output is structured uncertainty with a ranked attack plan.

## The Loop

1. Turn sources into evidence cards, one finding at a time.
2. Separate what a source observed from what its authors argued.
3. Map findings against competing theories.
4. Run study autopsies when credible sources conflict.
5. Score theories diagnostically, not as verdicts.
6. Use rotating adversarial roles to reduce fixation.
7. Generate research questions from unresolved conflict, missing undercuts, split scores, and scope flags.
8. Collect sources against thin cells in the coverage matrix.
9. Re-run the cycle on a cadence and keep prior uncertainty visible.

## What This Repo Contains

- `FIELD_NOTE.md`: the public field-note draft
- `templates/`: reusable Markdown templates for one manual cycle
- `examples/carverton/`: a fictional worked example using a city transit domain
- `examples/llm-benchmark-reliability/`: a small real-source pilot on benchmark interpretation
- `docs/for-autoresearch-builders.md`: bridge note for people building research loops
- `docs/pilot-use-cases.md`: candidate pilot domains and selection criteria
- `docs/adjacent-work.md`: nearby research areas and the novelty boundary
- `docs/what-this-is-not.md`: explicit limits and anti-overclaiming language
- `docs/release-notes.md`: v0.1 release notes and status

## Quick Start

Pick a contested field with at least two plausible theories and at least five sources that do not all point in the same direction.

Minimum first cycle:

1. Write two to four competing theory pages.
2. Create at least five evidence cards.
3. Run one autopsy on the clearest source conflict.
4. Generate three research questions from the artifacts.
5. Write a short cycle report naming what changed, what stayed unresolved, and what evidence should be collected next.

For that minimum pass, start with:

- `templates/theory-page.md`
- `templates/evidence-card.md`
- `templates/study-autopsy.md`
- `templates/research-question.md`

Use the other templates when the project needs a full cycle.

Full cycle:

1. Copy the files in `templates/` into a new project folder.
2. Write one theory page for each major explanation.
3. Create one evidence card per finding, not one per source.
4. Fill the `Conflicts with` field even when the answer is `none known`.
5. Run at least one study autopsy on a real or apparent conflict.
6. Score all theories in one session with the card deck open.
7. Generate research questions from the artifacts, not from intuition alone.
8. Collect the next sources against empty or thin matrix cells.

Do not treat the first cycle as a conclusion. Treat it as the first map of the disagreement.

## Human Review Boundary

This is a decision-support framework. It is not a decision-replacement system.

Human reviewers remain responsible for source selection, extraction quality, domain interpretation, safety boundaries, and any downstream decision. The templates are meant to make reasoning inspectable, not automatic.

## What This Is Not

This is not an autonomous scientist, a systematic review replacement, a truth machine, biomedical advice, or a benchmarked scientific-discovery engine. The full boundary is in `docs/what-this-is-not.md`.

## Status

v0.1. Markdown-only. No CLI, UI, package manager, automation, or live data extraction.
