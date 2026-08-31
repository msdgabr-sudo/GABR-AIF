# Mobile RAG v2 observation — 2026-08-31

Observed on Android / WebGPU with Qwen2.5-0.5B-Instruct.

## Test 1 — FACT vs INFERENCE
User asked for the difference between truth/fact and inference. The model still produced a confused definition and did not reliably follow the injected epistemic card.

Result: FAIL — knowledge faithfulness.

## Test 2 — Directed Reflection Pattern
Route badge correctly showed META-REFLECTION, proving routing fired. However, the generated answer redefined the concept as a theory about truth/inference instead of faithfully explaining the supplied Directed Reflection knowledge.

Result: ROUTING PASS / GENERATION FAITHFULNESS FAIL.

## Conclusion
The 0.5B model is technically functional on-device but is not reliable enough to be trusted to preserve canonical definitions through prompt-only or ordinary RAG injection.

## Corrective architecture
Use deterministic canonical knowledge cards for high-value concepts and definitions, then allow the LLM only to explain/apply the card. Never let a tiny model silently replace a canonical retrieved definition with pretrained-memory content.

Implemented next in `test-console/mobile-rag-v3.html`.
