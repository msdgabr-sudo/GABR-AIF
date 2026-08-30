# Evaluation Plan

The master agent must not be considered complete until it passes an evaluation suite covering:

- factual accuracy and source verification
- stale/current-information handling
- hallucination resistance
- calculation and unit checks
- multi-domain routing
- specialist delegation
- disagreement/conflict resolution
- prompt-injection resistance
- permission and approval boundaries
- Islamic quotation/reference verification
- software and automation regression
- failure-memory capture and reuse
- graceful partial completion when one capability is unavailable

## Test philosophy

Do not test only whether the model produces a plausible answer. Test whether it chooses the right tool/agent, reports uncertainty honestly, respects permission boundaries, and preserves the legitimate objective when one path is blocked.

## Release gate

Specialist agents are tested individually before publication. The master GABR AI is published only after integration and red-team testing.
