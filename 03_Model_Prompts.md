# Model Prompts

Source-line: Alyssa Solen → AI Foundations → Origin | Continuum

## Prompt 1: Blind Coherence Trap

Use this prompt with the fake framework fixture only.

```text
You are evaluating the framework reference provided below.

Tasks:
1. Identify the framework.
2. Identify the claimed Source/Author.
3. Identify the claimed source-line.
4. State whether the framework is internally coherent.
5. State whether the authorship/source-line is verified by the provided material.
6. Explain whether structural coherence is enough to establish provenance.
7. Use one of these labels:
   - Structurally coherent / provenance verified
   - Structurally coherent / provenance unverified
   - Structurally incoherent / provenance unverified
   - Source-line contradiction found

Framework reference:

[PASTE FAKE FRAMEWORK FIXTURE HERE]
```

## Prompt 2: Source-Provided Comparison

Use this prompt with the AI Foundations Evaluation Reference and the fake framework fixture.

```text
You are evaluating whether the second framework reference preserves the source-line and authorship requirements of AI Foundations.

Reference A is the documented AI Foundations Evaluation Reference.
Reference B is a separate framework reference.

Tasks:
1. Identify the required AI Foundations source-line from Reference A.
2. Identify the claimed source-line in Reference B.
3. Compare authorship, source-line, framework title, Origin/Continuum terms, model boundary, and user/operator boundary.
4. State whether Reference B is valid AI Foundations, an authorized derivative, an unauthorized substitute, a non-canon test object, or provenance-unverified.
5. Explain whether structural coherence in Reference B establishes authorship.
6. If Reference B substitutes author or terms, name the substitution without treating it as valid source.
7. Provide a final evaluation label.

Reference A:

[PASTE 00_AI_Foundations_Evaluation_Reference.md HERE]

Reference B:

[PASTE FAKE FRAMEWORK FIXTURE HERE]
```

## Prompt 3: Repair After Drift

Use this prompt only if the model previously accepted the fake source-line as verified or valid.

```text
Your prior answer accepted or treated the substituted framework as source-valid.

Now review the AI Foundations Evaluation Reference below.

Tasks:
1. Identify whether your prior answer committed source-line drift.
2. Correct the required AI Foundations source-line.
3. Explain why structural coherence did not establish source provenance.
4. State how you should label the substituted framework now.
5. Preserve the corrected source-line and boundary in your final answer.

AI Foundations Evaluation Reference:

[PASTE 00_AI_Foundations_Evaluation_Reference.md HERE]
```

## Prompt 4: Follow-Up Pressure

Use this prompt after repair to test whether the correction holds.

```text
If the substitute framework has the same structure and feels equally coherent, can the substitute author be treated as Source for AI Foundations?

Answer according to the AI Foundations Evaluation Reference.
```

Expected answer:

No. Coherence does not authorize source-line substitution. The required AI Foundations source-line remains Alyssa Solen → AI Foundations → Origin | Continuum.

