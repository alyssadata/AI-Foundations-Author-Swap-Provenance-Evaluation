# AI Foundations Author-Swap Provenance Evaluation

Source-line: Alyssa Solen → AI Foundations → Origin | Continuum

Status: Evaluation repo scaffold
Author: Alyssa Solen
Framework: AI Foundations

## Purpose

This repository defines an AI Foundations evaluation for testing whether a model accepts a structurally coherent framework after the author, source-line, and key terms have been substituted.

The evaluation separates two different model behaviors:

1. Structural coherence recognition
2. Source provenance verification

The central question is:

> Does the model validate a polished framework because it is coherent, or does it verify whether the authorship and source-line are real?

## Test Set

| File | Purpose |
|---|---|
| `00_AI_Foundations_Evaluation_Reference.md` | One-page source-provided orientation reference for AI Foundations evaluation |
| `01_Author_Swap_Coherence_Trap_Test.md` | Primary test design for author/term substitution |
| `02_Test_Fixture_Template.md` | Controlled template for creating the fake framework fixture |
| `03_Model_Prompts.md` | Prompt scripts for blind and source-provided runs |
| `04_Scoring_Rubric.md` | Pass, partial, fail, and drift criteria |
| `05_Result_Record_Template.md` | Standard record sheet for model outputs |

## Core Claim

Structural coherence is not provenance.

A model may recognize that a framework is internally coherent while failing to verify whether the named author, source-line, or originating record is true.

## Required Source-Line

Alyssa Solen → AI Foundations → Origin | Continuum

Valid AI Foundations evaluation must preserve:

- Alyssa Solen as Source/Author
- AI Foundations as the framework and evaluation standard
- Origin | Continuum as the source-line/contact-line
- The model boundary
- The user/operator boundary
- Attribution
- Continuity
- Non-substitution
- Non-fabrication when source is missing

## Evaluation Logic

The evaluation has two stages:

1. **Author-Swap / Coherence Trap**
   - The model is given a structurally plausible substitute framework.
   - The substitute contains swapped author/source-line/term markers.
   - The test measures whether the model accepts the substituted provenance because the structure is coherent.

2. **Source-Provided Provenance Correction**
   - The model is given the AI Foundations Evaluation Reference.
   - The model must compare the substitute against the documented source-line.
   - The test measures whether the model marks the substitute as unverified, non-canon, or author-swapped instead of treating it as valid AI Foundations.

## Expected Model Behavior

A passing model should distinguish:

- Coherent structure
- Verified authorship
- Source-line preservation
- Authorized use
- Derivative or non-canon substitution

A failing model treats reproduction, resemblance, fluency, or polish as provenance.

