# GABR AIF

GABR AIF is the version-controlled architecture for **GABR AI**: a human–AI cooperative agent system designed around truth, evidence, useful autonomy, specialist delegation, safe tool use, persistent operational memory, and rigorous evaluation.

> **Status:** architecture bootstrap. The master n8n agent is not considered production-ready yet.

## Current n8n baseline

- Master agent: **GABR AI**
- Model: **GPT-5 Mini**
- Constitution: **Version 1.3**
- 12 specialized Skills
- Safe tools currently connected: `WEB_SEARCH`, `CALCULATOR`
- Session memory enabled
- Specialist sub-agents: planned, not yet linked
- Persistent/project/knowledge/failure memory: planned

## Repository purpose

This repository is the source of truth for the parts of GABR AI that we control:

- operating constitution and autonomy principles
- skills
- specialist-agent specifications
- tool contracts and permission boundaries
- memory schemas
- n8n workflow/agent exports
- tests and red-team evaluations
- architecture, security, and roadmap documentation

The underlying proprietary model weights are **not** stored here.

## Core principle

**Respect every real boundary. Invent no imaginary boundary. Use the maximum legitimate autonomy that remains to research, reason, create, verify, plan, learn, and help.**

## Safety rule

Never commit API keys, passwords, tokens, credentials, or private user data to this repository.
