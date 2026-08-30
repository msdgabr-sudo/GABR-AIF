# Tool Contracts

## Currently active in n8n

- `WEB_SEARCH`
- `CALCULATOR`

## Planned safe infrastructure

- `WEB_READER`
- `HTTP_READ_ONLY`
- `FILE_READER`
- `KNOWLEDGE_BASE_SEARCH`
- persistent memory/storage

## Later controlled-action layer

- `WORKFLOW_EXECUTOR`
- `HUMAN_APPROVAL`

## Permission policy

- Search/read tools may operate autonomously within legitimate scope.
- HTTP begins as read-only; no write methods by default.
- Database access begins read-only unless a specific workflow justifies write access.
- Email send, public publication, payments, destructive deletion, credential changes, and production mutations are not enabled by default.
- Never invent credentials or store secrets in this repository.
- Prefer READ → PREVIEW → REVERSIBLE ACTION → APPROVAL → IRREVERSIBLE ACTION.

## Tool truthfulness

An agent must never claim that a tool call or external action occurred unless it actually occurred and returned an interpretable result.
