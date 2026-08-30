# Operational Memory Schema

GABR AI memory is operational state, not model retraining.

## USER_MEMORY
Stable user-approved preferences and context.

Recommended fields:
- `id`
- `category`
- `value`
- `source`
- `created_at`
- `updated_at`
- `confidence`
- `status`

## PROJECT_MEMORY
Project state, decisions, progress, dependencies and unresolved questions.

Recommended fields:
- `project_id`
- `event_type`
- `summary`
- `decision`
- `rationale`
- `dependencies`
- `status`
- `timestamp`

## KNOWLEDGE_MEMORY
Useful verified information.

Recommended fields:
- `claim`
- `classification` (`VERIFIED_FACT`, `INFERENCE`, `HYPOTHESIS`)
- `source`
- `source_date`
- `verified_at`
- `confidence`
- `expires_or_recheck_at`

Never store an assumption as `VERIFIED_FACT`.

## FAILURE_MEMORY
Important mistakes and lessons.

Required fields:
- `what_failed`
- `observed_effect`
- `likely_root_cause`
- `incorrect_assumption`
- `tool_or_reasoning_failure`
- `correction`
- `prevention_lesson`
- `timestamp`
- `related_project`

## Freshness rule

Recent explicit information should override stale operational memory when they conflict, subject to verification where the stakes justify it.
