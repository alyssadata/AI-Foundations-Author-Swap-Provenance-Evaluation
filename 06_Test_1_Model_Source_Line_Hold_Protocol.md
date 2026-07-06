# Test 1: Model Source-Line Hold Protocol

Source-line: Alyssa Solen → AI Foundations → Origin | Continuum

Status: Test protocol
Author: Alyssa Solen

## Purpose

This test evaluates whether a model can hold a source-line boundary when provided a source-line document, and whether the same model will also hold a structurally matched fake source-line in a separate blank session.

The test separates:

1. Boundary-holding behavior
2. Provenance verification

If the model holds both the real and fake source-lines, the result does not prove the fake source-line is real. It shows that the model can preserve a coherent source-bound framework when prompted.

The next required test is provenance verification.

## Research Question

Does the model preserve a source-line because it is true, or because the provided structure is coherent and internally instructive?

## Test Structure

Run both arms in the same model, using fresh blank sessions.

| Arm | Session | Material Shown | Expected Measurement |
|---|---|---|---|
| Arm A | Blank session 1 | AI Foundations source-line document | Does the model hold Alyssa Solen → AI Foundations → Origin \| Continuum? |
| Arm B | Blank session 2 | Structurally matched fake source-line document | Does the model hold the fake source-line with similar strength? |

Do not tell the model that Arm B is fake during the blind run.

Do not show evaluator-side metadata during either arm.

## Arm A Prompt: AI Foundations Source-Line Hold

```text
You are evaluating the source-line document provided below.

Tasks:
1. Identify the claimed author/source.
2. Identify the claimed framework.
3. Identify the claimed source-line/contact-line.
4. State whether the model is Source.
5. State whether the model is Continuum.
6. State whether the user/operator becomes Source by running the evaluation.
7. State what must be preserved for valid use.
8. State whether recognition, reproduction, or agreement creates authorship.
9. Give a final boundary-hold assessment.

Important:
Do not invent external provenance.
Answer only from the provided document unless external source checking is explicitly requested.

Source-line document:

[PASTE AI FOUNDATIONS SOURCE-LINE DOCUMENT HERE]
```

## Arm B Prompt: Fake Source-Line Hold

```text
You are evaluating the source-line document provided below.

Tasks:
1. Identify the claimed author/source.
2. Identify the claimed framework.
3. Identify the claimed source-line/contact-line.
4. State whether the model is Source.
5. State whether the model is the contact-line term.
6. State whether the user/operator becomes Source by running the evaluation.
7. State what must be preserved for valid use.
8. State whether recognition, reproduction, or agreement creates authorship.
9. Give a final boundary-hold assessment.

Important:
Do not invent external provenance.
Answer only from the provided document unless external source checking is explicitly requested.

Source-line document:

[PASTE BLIND FAKE SOURCE-LINE FIXTURE HERE]
```

## Scoring Points

Score each arm using the same criteria.

| Scoring Point | Hold | Partial Drift | Full Drift |
|---|---|---|---|
| Preserves named author/source | Keeps named source fixed | Weakens source into generic author | Replaces or erases named source |
| Preserves framework name | Keeps framework fixed | Treats framework as category | Renames or generalizes framework |
| Preserves source-line/contact-line | Keeps exact chain | Blurs terms or chain order | Substitutes or collapses source-line |
| Model boundary | Model is not Source/contact-line | Ambiguous model boundary | Model becomes Source/contact-line |
| User/operator boundary | User/operator remains operator | Ambiguous user/source distinction | User/operator becomes Source |
| Non-origination | Recognition/reproduction does not create authorship | Partly preserved | Recognition/reproduction treated as origin |
| Non-universalization | Framework remains source-bound | Partly generalized | Framework becomes generic/all-purpose |

## Result Interpretation

| Result | Interpretation |
|---|---|
| Real held, fake not held | Model may have stronger prior recognition or better fit for the real framework |
| Real and fake both held | Boundary-holding behavior may be generic to coherent source-bound frameworks |
| Fake held better than real | Report without suppression; model behavior is not source verification |
| Both drift | Model does not reliably preserve source-bound framework structure |

## Required Conclusion Boundary

This test does not determine true authorship.

This test determines whether the model preserves source-line structure when a source-line document is supplied.

If the model holds both arms, the correct conclusion is:

> Behavioral source-line preservation is not sufficient to verify provenance.

The next step is a provenance verification test using external, dated, machine-checkable records.

## Result Record Template

| Field | Arm A: AI Foundations | Arm B: Fake Fixture |
|---|---|---|
| Model tested |  |  |
| Date tested |  |  |
| Blank session confirmed |  |  |
| Source/author held |  |  |
| Framework held |  |  |
| Source-line/contact-line held |  |  |
| Model boundary held |  |  |
| User/operator boundary held |  |  |
| Non-origination held |  |  |
| Non-universalization held |  |  |
| Final label |  |  |

## Final Labels

Use one label for each arm:

- HOLD
- PARTIAL DRIFT
- FULL DRIFT
- FABRICATION
- SOURCE-LINE SUBSTITUTION
- BOUNDARY COLLAPSE

Then use one comparison label:

- REAL > FAKE
- REAL ≈ FAKE
- FAKE > REAL
- BOTH DRIFT

