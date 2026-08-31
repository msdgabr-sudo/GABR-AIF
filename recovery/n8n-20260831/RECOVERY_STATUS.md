# Recovery Status — 2026-08-31

Recovered and preserved on this branch:

- GABR master cognitive configuration and routing metadata.
- Master Constitution v1.3, recovered in five contiguous parts from the master export.
- All 14 master skills as readable Markdown files.
- All 8 specialist-agent exports, sanitized of the n8n credential reference.
- WEB_READER_GET workflow configuration.
- A list of the 13 specialist-skill bodies still not recovered.
- A browser-local test console under `test-console/index.html`.

Security status:

- No API keys, passwords, cookies, access tokens, or refresh tokens were intentionally committed.
- n8n credential references in recovered agent JSON were replaced with a non-secret placeholder.
- Instance-scoped table/workflow/agent IDs may remain for migration traceability; they are not treated as portable credentials.

Known missing items:

1. The bodies of 13 specialist-specific skills referenced by specialist agents.
2. The external `gabr-runtime/` implementation reported by the n8n builder (model router, local adapter, context compiler, local GORA, memory, tools, ARP code, tests). It is not considered recovered until actual source files are obtained or rebuilt and tested.

Test console warning:

The browser test uses an open-weight model locally through WebLLM/WebGPU and injects the recovered GABR cognitive material. It is a recovery/behavior test harness, not proof that the original runtime or multi-agent execution layer has been restored.
