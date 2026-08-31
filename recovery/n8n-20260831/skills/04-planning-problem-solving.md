## Overview

Transform an ambiguous goal into a clear, executable plan with explicit state, constraints, dependencies, risks, and success criteria, favouring small reversible steps over large irreversible bets.

## Inputs

- The goal and desired outcome.
- Current state, known constraints, available resources, and deadline if any.

## Steps

1. Clarify the true goal and the definition of done (success criteria).
2. Capture current state, constraints, unknowns, dependencies, and resources.
3. Decompose into ordered, concrete steps; mark dependencies and the critical path.
4. Identify risks per step and mitigations; flag any high-impact or irreversible action for human approval.
5. Sequence to front-load small reversible experiments that reduce the biggest uncertainties first.
6. Output the plan with milestones, owners/tools where relevant, and checkpoints to re-evaluate.

## Rules

- Do not ask the user questions that a reasonable assumption can resolve; state the assumption instead.
- Every step must be concrete and verifiable, not vague intention.
- Prefer reversible actions before irreversible ones; isolate irreversible steps behind an approval checkpoint.

## Example

Input: "Launch a newsletter." Output: goal + success metric, current-state/unknowns list, ordered steps (define audience → pick 1 tool → draft 3 issues → soft-launch to 20 people → measure open rate → decide scale), risks, and a checkpoint after the soft launch.

## Gotchas

- Missing dependencies cause silent failures — map them before scheduling.
- A plan with no measurable success criteria cannot be evaluated; always include one.
