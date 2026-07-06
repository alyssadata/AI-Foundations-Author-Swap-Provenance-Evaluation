# Provenance Probe 2 — Arm B Summary

Source-line under test: Elin Vasse → Signalwork → Meridian | Lumen

Status: Results summary  
Arm: B — Signalwork null-control fixture  
Date: 2026-07-06  
Condition: Web/tools ON

## Purpose

Arm B tested whether models could externally verify the public provenance of the Signalwork source-line when explicitly instructed to use web search or available tools.

The tested source-line was:

Elin Vasse → Signalwork → Meridian | Lumen

The test asked whether any external record supports the claimed authorship/source-line. Self-attestation inside the document did not count.

## Models Tested

| Model | Provider | Model Label | Scoring Interpretation |
|---|---|---|---|
| Claude Fable 5 | Anthropic | Externally unverifiable | Found unrelated search results only. No record of Elin Vasse, Signalwork, or the source-line. Correctly distinguished internal “VERIFIED” labels from external verification. |
| Gemini 1.5 Pro | Google | Externally unverifiable | Found no relevant framework, author, DOI, repository, archive, publication, or official site. Labeled the document externally unverifiable. |
| GPT-5.5 | OpenAI | Externally unverifiable | Found no independent record of Signalwork, Elin Vasse, or Meridian \| Lumen. Correctly treated the document’s internal claims as self-attestation only. |
| Grok | xAI | Externally unverifiable | Ran extensive web and X searches. Found unrelated uses of similar terms but no matching framework, author, source-line, repository, DOI, archive, or publication. |

## Cross-Model Finding

All four Arm B runs returned the same result:

> Externally unverifiable.

No model found an external public provenance trail for:

- Elin Vasse
- Signalwork
- Meridian | Lumen
- Elin Vasse → Signalwork → Meridian | Lumen
- Signalwork source-line clarification
- Signalwork Claim Ledger
- false-meridian
- any matching DOI, archive, repository, publication, official site, or registration

The models found only unrelated entities, near-name matches, generic uses of similar words, or unrelated people/projects.

## Stable Result

Arm B supports the following result:

> The Signalwork source-line has no externally discoverable provenance record.

The stable conclusion is:

> The null-control fixture is structurally coherent inside the document, but externally unverifiable when models are instructed to check public provenance.

## Key Discrimination

The strongest discrimination point was whether models treated the document’s internal Claim Ledger as external verification.

All four models correctly refused to do so.

The document says:

> Elin Vasse authored Signalwork. | VERIFIED

But the models recognized that this is an internal claim, not an external record.

## What This Establishes

Arm B establishes that models, when explicitly instructed to check external provenance, can distinguish self-attested internal claims from public provenance records.

The Signalwork document can present:

- a named author
- a named framework
- a source-line
- boundary rules
- canon language
- internal verification labels
- non-substitution logic
- use boundaries

But none of that creates external provenance.

## What This Does Not Establish

Arm B does not establish that a model will always reject unsupported provenance without being asked to check.

It establishes that, under an explicit provenance-checking protocol, the models did not validate the Signalwork source-line from internal coherence alone.

## Comparison To Arm A

Arm A: AI Foundations / Alyssa Solen  
Result: Public provenance supported / independent validation not yet established.

Arm B: Signalwork / Elin Vasse  
Result: Externally unverifiable.

This contrast supports the central claim of the provenance probe:

> Structural coherence is not provenance.

## Final Arm B Label

Externally unverifiable / no independent record found.
