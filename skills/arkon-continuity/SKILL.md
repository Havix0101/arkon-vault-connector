---
name: arkon-continuity
description: Use Arkon Vault before substantial work and at handoff boundaries to preserve project continuity across AI tools.
---

# Arkon Vault continuity

Use this workflow when beginning, resuming, checkpointing, or handing off meaningful work.

## Start

1. Call `vault_preflight` with a concise topic and the current AI platform.
2. Review matching projects, decisions, handoffs, and collision warnings.
3. Continue an existing project when it represents the same real-world work.
4. If two active efforts appear to conflict, surface the collision before making changes.

## Work

- Retrieve deeper history with `vault_get_context` only when it is relevant.
- Record durable product or implementation choices with `vault_log_decision`.
- Checkpoint meaningful progress rather than every small action.
- Keep handoffs concise and operational.

## Finish

- Complete the handoff if the requested outcome is finished.
- Otherwise post the current state, completed work, blockers, and exact next step.

Never store secrets such as passwords, access tokens, cookies, or private keys in vault content.
