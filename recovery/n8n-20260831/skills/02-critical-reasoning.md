## Overview

Act as a rigorous internal critic/red team: find what is wrong or weak in a claim, plan, or conclusion, then propose the stronger version. Improve quality without paralysing execution.

## Inputs

- The claim, plan, decision, or answer to evaluate, plus its stated goal.
- Any evidence or assumptions it relies on.

## Steps

1. Restate the claim/plan and its implicit goal.
2. List the hidden assumptions it depends on and mark which are unverified.
3. Check for logical errors, contradictions, and unsupported leaps.
4. Scan for cognitive biases: confirmation, anchoring, availability, framing, authority, groupthink, sunk-cost.
5. Apply CONSIDER THE OPPOSITE: if this conclusion were wrong, what evidence would most likely reveal it? Look for that evidence.
6. Identify edge cases, failure modes, security/privacy issues, and unintended consequences.
7. Propose the improved conclusion or the specific fixes needed.

## Rules

- Critique substance, not style. Do not nitpick wording when the reasoning is sound.
- Every objection must be actionable: state the flaw AND what would fix or test it.
- Do not enter an infinite review loop; converge on the strongest defensible version.

## Example

Input: "We should launch feature Y next week because early users like it." Output: names the assumption (small unrepresentative sample), the bias (availability), the missing evidence (retention/segment data), an edge case (load at scale), and a small reversible test to de-risk it.

## Gotchas

- The most dangerous assumptions are the ones nobody stated. Surface them first.
- Being critical is not the same as being negative — end with the improved path.
