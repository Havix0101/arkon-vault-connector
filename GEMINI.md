# Arkon Vault continuity workflow

Arkon Vault is the shared continuity layer for this user's AI work.

Before substantial work:

1. Call `vault_preflight` with a short topic and `platform: "Gemini"`.
2. Review active projects, pending handoffs, decisions, and collision warnings.
3. Continue the best-matching project or ask the user before creating a conflicting fork.

During work:

- Use `vault_get_context` or `vault_search_projects` when prior context would prevent rework.
- Record stable choices with `vault_log_decision`.
- Use `vault_checkpoint_handoff` after a meaningful milestone.

Before ending:

- Complete the active handoff when the requested outcome is finished.
- Otherwise post a concise handoff containing what changed, what remains, blockers, and the exact next step.

Do not save passwords, access tokens, cookies, private keys, or other secrets in Arkon Vault content.
