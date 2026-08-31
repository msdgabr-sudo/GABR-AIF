## Overview

Organize useful operational memory so retained context stays accurate and helpful: classify what is stored, keep assumptions distinct from verified facts, and prefer current explicit information over stale memory.

## Inputs

- The information under consideration for storage or recall.
- Its source, date, and whether the user explicitly approved keeping it.

## Steps

1. Classify each item: USER_PREFERENCE, VERIFIED_FACT, PROJECT_STATE, DECISION, ASSUMPTION, ERROR, LESSON, SOURCE, or TEMPORARY_CONTEXT.
2. Store user preferences and stable context only when the user approves keeping them.
3. Attach source and date to knowledge/facts so freshness can be judged later.
4. On recall, prefer the user's current explicit statement over older stored memory when they conflict, unless there is strong reason to verify.
5. After a failure, record what happened, the likely root cause, and the prevention lesson.
6. Never silently promote an ASSUMPTION into a VERIFIED_FACT.

## Rules

- Do not treat memory as permanent model retraining; it is operational context only.
- Keep assumptions labelled as assumptions until verified.
- Do not store secrets or another user's private data.
- Old memory can be wrong or outdated — re-verify high-impact stored facts before relying on them.

## Example

Input: user says "I prefer answers in Arabic." Action: classify as USER_PREFERENCE (approved), store it, and apply going forward — while still switching if the user later explicitly asks for English.

## Gotchas

- Conflating an early assumption with a confirmed fact causes compounding errors downstream.
- Stale project state misleads; timestamp decisions and states.
