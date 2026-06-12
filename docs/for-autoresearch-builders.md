# For Autoresearch Builders

This project is for the cases where an autoresearch loop cannot rely on a clean scoreboard.

Many successful autoresearch setups have a tight loop:

1. propose a change
2. run the experiment
3. read the score
4. keep or reject the change
5. repeat

That loop works when the environment gives useful feedback. A validation curve, benchmark score, simulation result, test suite, or attack-success rate can act as the scoreboard.

Some research domains do not have that. The disputed object may be the construct, the scope condition, the causal mechanism, or the standard of evidence. In those settings, optimizing directly for confidence can reward the wrong behavior.

## The Core Translation

Contested Evidence Autoresearch treats the research state as a structured evidence workspace.

| Autoresearch concept | This field kit |
| --- | --- |
| State | Evidence deck, theory map, conflict graph, question backlog, source coverage matrix |
| Action | Card a source, autopsy a conflict, sharpen a theory, add an undercut, generate a question, collect against a thin cell |
| Feedback | Better source traceability, clearer conflicts, stronger scope discipline, more vulnerable theories, higher-value next questions |
| Failure mode | Premature convergence on a confident answer |
| Human gate | Reviewers validate cards, scope claims, autopsies, and downstream conclusions |

The point is not to make the loop autonomous. The point is to make the loop inspectable.

## What Can Be Automated

The loop has automatable transitions, even though v0.1 is manual-first.

| Transition | Possible automation | Human gate |
| --- | --- | --- |
| Source to card | Draft a finding card from a source passage | Reviewer confirms the finding sentence, scope, strength grade, and source link |
| Card to conflict | Suggest cards that appear to disagree | Reviewer decides whether the conflict is real, apparent, or out of scope |
| Conflict to autopsy | Draft an autopsy across construct, scope, time, method, analytic flexibility, and unresolved conflict | Reviewer assigns the category and records what would resolve it |
| Theory map to question | Identify missing undercuts, untested distinctive predictions, and scorer splits | Reviewer approves the question and pre-commitment |
| Question to collection plan | Suggest searches, source types, and thin matrix cells | Reviewer checks feasibility, source quality, and safety boundaries |

The useful automation target is not "choose the answer." It is "make the next reviewable research move cheaper and easier to inspect."

## What The Loop Optimizes

This loop does not optimize a single scalar objective.

It optimizes practical evidence quality:

- claim-evidence binding
- separation of finding from interpretation
- conflict visibility
- theory vulnerability
- scope specificity
- independence of support
- next-question discrimination power

The closest thing to reward is not "the theory won." It is "the next cycle has fewer hidden assumptions and better questions."

## Why This Matters For Autoresearch

Autoresearch systems are credible when their feedback signal is credible.

When the feedback signal is weak, ambiguous, delayed, or socially constructed, the loop needs a different target. It should first improve the evidence environment it is reasoning inside.

This field kit proposes one manual-first version of that target. The templates are the state format. The loop is the protocol. Automation can be added only where the artifact produced can still be reviewed.

## Candidate Uses

Good fits:

- deciding whether a benchmark result supports a broad capability claim
- comparing competing explanations for an eval failure
- mapping uncertainty around an AI safety claim
- planning what evidence to collect before building a new benchmark
- organizing mixed literature before a more formal review

Poor fits:

- hyperparameter search with a clean validation metric
- benchmark optimization where the score is trusted
- executable experiments with clear pass/fail results
- domains requiring formal systematic review from the start
- safety-critical decisions without accountable domain governance

## Minimal Builder Experiment

Try the kit on one contested research claim.

Example shape:

1. Choose one claim: "Benchmark X measures capability Y."
2. Write three theories:
   - the benchmark validly measures Y
   - the benchmark mostly measures test familiarity or contamination
   - the benchmark measures a narrower subskill than claimed
3. Create five evidence cards from primary benchmark papers, critique papers, and evaluation reports.
4. Run one autopsy on a source conflict.
5. Generate three questions that would move confidence.
6. Decide whether the next useful move is a test, a literature pass, a benchmark audit, or a scope correction.

If the loop ends with a narrower claim and a better experiment, it worked.

## Design Boundary

This is not a proposal to replace benchmarked autoresearch. If a clean scoreboard exists and is trusted, use it.

This is for the layer before that: the layer where the team decides whether the scoreboard actually measures the thing it is being asked to measure.
