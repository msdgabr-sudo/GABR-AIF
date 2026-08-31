# GABR AIF n8n Recovery Snapshot — 2026-08-31

This directory preserves the portable cognitive configuration recovered from the expiring n8n environment.

Included now:
- Master agent export (sanitized)
- 8 specialist-agent exports (sanitized)
- Master Constitution v1.3 recovered from the master export
- 14 master skills recovered from the n8n configuration / pasted skill content
- WEB_READER_GET workflow export
- Master skill-ID map (mapping marked as inferred where names are not embedded in the master export)
- Specialist skill references that are still missing and should be recovered separately

Security:
- n8n credential references were removed from uploaded agent JSON.
- No API keys, passwords, cookies, or tokens are intentionally included.
- Instance-scoped non-secret IDs are preserved only to help migration tracing.

Important limitation:
The external `gabr-runtime/` code reported by the n8n builder is NOT present in this recovery snapshot unless separately recovered. This snapshot preserves the cognitive/configuration layer, not proof of the external runtime implementation.
