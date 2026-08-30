# n8n Integration

## Status

n8n Cloud is a **temporary prototyping environment**, not a required production dependency for GABR AIF.

The user does not intend to subscribe to n8n Cloud after the current access period ends. Therefore all work must be designed for migration and portability.

## What must be captured before n8n Cloud access ends

- exported agent/workflow JSON where available
- sanitized configuration snapshots
- GABR AI master instructions/constitution
- all 12 Skill definitions
- specialist-agent definitions
- routing/delegation logic
- tool descriptions/contracts
- memory design
- test prompts and observed results

## Secrets policy

Never export or commit credentials, API keys, tokens, cookies, private user data, or environment-specific secrets. Replace sensitive values with placeholders and document required environment variables separately.

## Migration targets

### Option A — self-hosted n8n Community Edition
n8n provides a standard self-hosted Community Edition. This can be used without an n8n Cloud subscription and can run locally with Docker. It remains an optional runtime/migration aid rather than a permanent product dependency.

### Option B — standalone GABR AIF runtime
The preferred long-term architecture is an independent backend stored in this repository with:
- orchestrator
- specialist-agent router
- tool registry
- persistent memory
- model-provider abstraction
- secure API for the GABR AIF app

This makes the project portable across model providers and automation engines.

## Current external baseline

The temporary live n8n Cloud master currently uses GPT-5 Mini, Constitution v1.3, 12 Skills, WEB_SEARCH, CALCULATOR, and session memory.

Before the cloud instance expires, treat it as a prototype to harvest and validate design—not as the final home of GABR AIF.
