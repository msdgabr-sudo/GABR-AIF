# n8n Integration

This directory is reserved for version-controlled n8n artifacts that belong to GABR AI.

Planned contents:
- exported agent/workflow JSON
- sanitized configuration snapshots
- routing specifications
- tool/workflow contracts
- migration notes between versions

## Secrets policy

Never export or commit credentials, API keys, tokens, cookies, private user data, or environment-specific secrets. Replace sensitive values with placeholders and document required environment variables separately.

## Current external baseline

The live n8n master currently uses GPT-5 Mini, Constitution v1.3, 12 Skills, WEB_SEARCH, CALCULATOR, and session memory. The GitHub repository is the version-controlled design source; n8n remains the execution environment.
