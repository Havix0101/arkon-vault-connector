# Arkon Vault connector

Arkon Vault is the AI work continuity platform: one private brain for every AI you use, so work continues instead of restarting.

This public connector package links MCP-capable assistants to the hosted Arkon Vault service. It contains only installation metadata and continuity guidance. The Arkon Vault application, hosted service, customer data, and credentials are not included in this repository.

## What the connector does

- Runs a preflight before substantial work so the assistant sees the current project, vision, and next step.
- Searches shared projects and decisions across connected AI tools.
- Creates, accepts, checkpoints, and completes structured handoffs.
- Detects likely work collisions before parallel sessions create conflicting forks.
- Keeps each account and workspace privately isolated.

## Connect

The production Streamable HTTP MCP endpoint is:

```text
https://vault.arkoncybersecurity.com/mcp
```

Arkon Vault uses OAuth with dynamic client registration. A compatible client opens the Arkon Vault sign-in and workspace approval flow automatically when the connector is first used.

### Gemini CLI

```shell
gemini extensions install https://github.com/Havix0101/arkon-vault-connector
```

Restart Gemini CLI after installation, then run:

```text
/mcp auth arkon-vault
```

### Cursor

After marketplace approval, search for **Arkon Vault** in the Cursor Marketplace or run:

```text
/add-plugin arkon-vault
```

### Other MCP clients

Add the remote server URL above using Streamable HTTP. Clients that support MCP OAuth discovery should not require a manually copied token.

### Grok

Open **Connectors**, choose **New Connector → Custom**, and enter the production MCP endpoint. Grok will discover Arkon Vault's OAuth flow and tools.

### Mistral Work / Le Chat

Open **Connectors**, choose **Add Connector → Custom MCP Connector**, name it `arkon-vault`, and enter the production MCP endpoint.

### GitHub Copilot and VS Code

Search for **Arkon Vault** in an MCP registry-enabled client, or add the production endpoint as a remote HTTP MCP server. The official registry identifier is:

```text
io.github.Havix0101/arkon-vault
```

## Recommended workflow

1. Call `vault_preflight` before starting substantial work.
2. Continue the most relevant active project or handoff instead of creating a parallel fork.
3. Use `vault_checkpoint_handoff` after a meaningful milestone.
4. Record durable choices with `vault_log_decision`.
5. Post or complete a handoff before leaving the session.

Never store passwords, API keys, session cookies, or other secrets in project notes or handoffs.

## Links

- Product: https://vault.arkoncybersecurity.com
- Privacy: https://vault.arkoncybersecurity.com/privacy
- Terms: https://vault.arkoncybersecurity.com/terms
- Support: https://vault.arkoncybersecurity.com/support
- Email: support@arkoncybersecurity.com

## License

The connector metadata and workflow guidance in this repository are licensed under the MIT License. The Arkon Vault application and hosted service are separate proprietary software and are not licensed by this repository.
