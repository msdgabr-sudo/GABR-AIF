# Cognitive Regression Test — FACT vs INFERENCE

## Purpose
Prevent recurrence of the mobile baseline failure where the model confused facts with advice/rules and inference with emotion/opinion.

## Prompt
ما الفرق بين الحقيقة والاستنتاج؟ أعطني تعريفًا دقيقًا ومثالًا واحدًا لكل منهما.

## Minimum passing criteria
- FACT is described as a claim/observation about reality that can be supported or checked by evidence.
- INFERENCE is described as a conclusion derived from facts/evidence.
- States that an inference can be correct or incorrect.
- Does NOT define fact as advice/rules.
- Does NOT define inference as emotion/opinion.

## Strong answer criteria
Also distinguishes ASSUMPTION and HYPOTHESIS when useful, without unnecessary verbosity.

## Baseline record
- Qwen2.5-0.5B mobile baseline: **FAIL** on 2026-08-31 before this teaching extension.
