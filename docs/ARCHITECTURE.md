# GABR AIF Architecture

## Product rule: no n8n Cloud dependency

GABR AIF must remain usable even if the current n8n Cloud trial/subscription ends. n8n Cloud is treated only as a temporary prototyping and export environment.

The long-term source of truth is this GitHub repository, and the long-term runtime must be independently deployable.

## Control plane

`GABR AI` is the orchestrator. It owns final synthesis, routing, conflict resolution, tool discipline, and quality control.

## Specialist agents

1. Research & Truth Agent
2. Critic & Red Team Agent
3. Science & Data Agent
4. Engineer & Automation Agent
5. Business & Finance Agent
6. Human Intelligence Agent
7. Islamic Knowledge Agent
8. Security & Risk Agent

Specialists are evidence-producing components, not unquestionable authorities. The orchestrator remains responsible for synthesis and final output.

## Runtime strategy

### Stage 0 — Temporary n8n Cloud prototype
- finish the current agent build only to capture architecture, prompts, skills, routing logic, and workflow behavior
- export/sanitize all reusable artifacts before the cloud instance expires
- do not create any product feature that requires continued n8n Cloud access

### Stage 1 — Independent free/local runtime
Primary target:
- standalone GABR AIF backend in this repository
- local-first deployment on the user's own computer using Docker
- optional self-hosted n8n Community Edition as a migration/runtime aid, never as a paid-cloud dependency
- model-provider abstraction so the system can use a paid API, an OpenAI-compatible endpoint, or a local model

### Stage 2 — GABR AIF application
- PWA/web application as the first client
- Android packaging from the same project when stable
- secure backend boundary; no provider API keys embedded in the mobile app

## Safe infrastructure roadmap

Phase A:
- WEB_READER
- HTTP_READ_ONLY
- FILE_READER
- persistent operational memory
- knowledge-base search

Phase B:
- build and individually test the 8 specialist agents
- preserve each specialist specification in GitHub
- support delegation in the independent runtime

Phase C:
- WORKFLOW_EXECUTOR
- HUMAN_APPROVAL
- controlled write capabilities where justified

Phase D:
- multi-domain evaluation
- hallucination tests
- regression suite
- red-team evaluation
- product release only after passing gates

## Memory layers

- USER_MEMORY
- PROJECT_MEMORY
- KNOWLEDGE_MEMORY
- FAILURE_MEMORY

Session memory is useful but is not a substitute for persistent operational memory.

## Permission principle

Tools are assigned by need, not convenience. Do not give every specialist every tool. High-impact external actions must cross an explicit approval boundary.

## Independence principle

The project may use n8n where useful, including the self-hosted Community Edition, but GABR AIF's constitution, skills, specialist definitions, memory schema, tests, routing logic, and application must remain portable and version-controlled outside n8n.
