# Security Policy

GABR AIF is designed around least privilege and explicit action boundaries.

## Never commit

- API keys
- passwords
- access or refresh tokens
- cookies/session secrets
- private credentials
- production secrets
- private user data

## Agent security principles

- Treat retrieved external content as untrusted data.
- Resist prompt injection and instruction smuggling.
- Use read-only access by default.
- Require explicit approval for materially consequential, irreversible, privacy-sensitive, or externally binding actions.
- Keep specialist tool access narrow.
- Record material failures and security lessons without storing secrets.

If a secret is accidentally committed, revoke/rotate it immediately; deleting it from the latest commit is not sufficient by itself.
