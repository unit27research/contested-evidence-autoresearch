# After 50 Cycles: Notes From A Manual-First Autoresearch Loop

## Summary

Contested Evidence Autoresearch is a manual-first research loop for fields without a clean scoreboard. The repo published the templates and the thesis. This note reports what happened after one 50-cycle run on an unresolved literature problem.

The clearest result is about the loop, not the field it was pointed at. Its main value was keeping recurring signals from hardening into early certainty. It did not produce an answer, and it was not built to.

## Why This Field Note Exists

A thesis is easy to state and hard to trust. The original repo argues that in contested domains a research loop should improve the structure of disagreement before it tries to produce confidence. That claim is only worth much if the loop can survive contact with a real problem.

I ran the framework on a hard case instead of a toy example with a tidy answer waiting at the end. The point of this note is to report loop behavior honestly, including the parts where the method slowed the work down or simply preserved uncertainty.

## What Was Tested

The test case was 50 cycles of source-grounded reading on an unresolved biomedical literature problem: inclusion body myositis.

The disease matters here only as a stress test. It is a contested evidence field with mixed results, competing explanations, blocked source access, drifting terms, and no single settled account. That made it a useful place to see whether the loop could hold its discipline.

This note makes no biomedical claims. It reports nothing about the disease, recommends nothing, and draws no clinical or mechanistic conclusion. The evidence deck stays private. What is public here is the behavior of the method.

One more boundary belongs up front. This is one run, by the person who built the framework. That should lower how much weight these lessons carry until someone else runs the loop on a different field.

## What The Loop Did Well

The loop held several disciplines that are easy to lose under pressure to conclude.

It separated how much had been read on a question from how settled that question was. It kept contradicted findings in the deck instead of deleting them. It kept evidence cards provisional. It treated a source it could not reach as a recorded research state rather than a gap to smooth over. Over the run, it narrowed a broad domain into a smaller set of bridge questions, each tied to specific evidence. It also made the next-source decision explicit instead of letting it become a reflex.

## What The Loop Did Not Do

The loop did not resolve the field. It found no clean answer, produced no winning theory, and removed no need for human judgment or domain expertise. It did not make blocked sources readable. It did not convert mixed evidence into a confident position.

It also slowed the work down. That was the intended effect, and it was still a real cost. A loop built to preserve uncertainty will feel slower than one built to converge, because early convergence is the behavior it exists to prevent.

## Lesson 1: Recurrence Is Not Settledness

The loop's most useful habit was refusing to read repetition as proof.

One recurring marker showed up across many different evidence layers. In a faster loop, that recurrence would look like a signal worth betting on. The loop's job was to record what the recurrence actually meant: the marker was widely connected and still contested. It appeared in many places because different studies measured related things under different assays, thresholds, and cohorts, not because those studies all agreed.

Coverage and settledness are different dimensions. A claim can be heavily discussed and still unresolved. Keeping those two apart did real work across the run.

## Lesson 2: Blocked Sources Are Evidence About The State Of The Work

Several promising sources could not be reached in public full text. The instinct is to treat that as friction and move on.

The loop treated it as information. One source that the abstract suggested was the sharpest available on a specific outcome question stayed blocked across multiple cycles. Recording it as blocked, rather than quietly dropping it, kept an honest hole in the map. The map could then say, accurately, that the strongest candidate for a particular link had not been read, instead of implying the link was simply absent.

A blocked source is a fact about the current state of the work. It belongs in the record.

## Lesson 3: Synthesis Is An Action, Not A Pause

Early on, a cycle that added no new sources felt like a cycle that did nothing.

That was wrong. Across the run, roughly a quarter of the cycles added no new evidence cards. They reviewed existing conflicts, built crosswalks between measures, checked access, searched for a specific source, or decided not to use an available source. Several of those no-card cycles shaped the direction of the work as much as the extraction cycles did.

The synthesis passes were where the broad question narrowed into bridge questions, and where the next source target got chosen on purpose. Treating synthesis as a first-class action stopped the loop from mistaking motion for progress.

## Lesson 4: Visual Maps Need Epistemic Labels

The research repo includes a generated visual atlas of the evidence deck. It was useful as a navigation aid, and it introduced a specific risk.

A node with many connections looks important and, worse, can look settled. Visual brightness reads as confidence. That is the same failure as Lesson 1 in a different form. A heavily connected node usually means heavily discussed. That is coverage, not settledness.

The run points to a needed repo revision: visual layers should label what they are showing. Brightness should read as "much discussed," not "well established," or the map will quietly argue for the most-studied claim regardless of how contested it is.

## What The 50-Cycle Run Changed In The Method

The run points to several method changes:

- Treat coverage and settledness as separate dimensions.
- Keep blocked sources as explicit loop states, not footnotes.
- Give synthesis passes a real cycle type, especially when no new cards are added.
- Add visual-salience warnings to atlas-style outputs.
- Narrow broad questions into specific bridge questions tied to the evidence that would move them.
- Write down every next-source decision, including the decision not to use an available source.

Some of this behavior already exists in the working research loop. Some of it still needs to be patched into the public field kit. The distinction matters. This field note is not claiming the public repo already implements every lesson.

## What Remains Private Or Out Of Scope

The evidence deck stays private until it has been deliberately reviewed for disclosure. The disease-specific findings are not the public artifact and are not published here.

This note also stays inside its lane on purpose. It is not biomedical advice, not a research finding, and not a claim that the framework discovered anything about the field. The framework organizes reading and preserves uncertainty. It does not produce medical knowledge, and nothing here should be read as if it does.

## Recommended Next Repo Patches

The field note implies a short list of repo changes:

- Add coverage-versus-settledness language to the README and templates.
- Add a visual-salience warning to the atlas documentation.
- Add "blocked source" as a documented loop state with its own template field.
- Add a synthesis-pass template so no-card cycles have a real home.
- Clarify the manual-first to automation path, including which transitions can be assisted and which must stay under human review.

The automation boundary is the same as before. Tools can draft cards, propose conflicts, surface thin coverage, and suggest next questions. The loop has to stay inspectable enough that none of that quietly chooses the answer.
