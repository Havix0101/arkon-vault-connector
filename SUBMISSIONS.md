# Universal connector distribution status

Last updated: 2026-07-30

| Surface | Status | Distribution path |
|---|---|---|
| Official MCP Registry | Live | `io.github.Havix0101/arkon-vault` version `1.6.0` |
| Public connector repository | Live | `https://github.com/Havix0101/arkon-vault-connector` |
| Google terminal AI | Direct MCP ready | Google moved individual terminal users to Antigravity CLI, which migrates MCP settings; eligible enterprise/API-key users can still use the Gemini CLI extension directly |
| GitHub Copilot / registry-aware MCP clients | Eligible | The official MCP Registry entry provides the remote Streamable HTTP endpoint |
| Cursor Marketplace | Review pending | Marketplace application submitted; wait for a provider decision or feedback |
| MCP.so remote directory | Package ready | Account sign-in and free queued submission remain |
| Smithery | Package ready | Publisher sign-in and authenticated server scan remain |
| Grok | User-installable | Grok supports the production endpoint as a Custom MCP connector; no public catalog submission process is documented |
| Mistral Work / Le Chat | User-installable | Mistral supports the production endpoint as a Custom MCP Connector; no public directory submission process is documented |
| Windsurf | User-installable | Windsurf supports the production Streamable HTTP endpoint; no public publisher application was found |
| Microsoft Copilot | Technically compatible | Public commercial distribution requires a separate Partner Center / AppSource seller workflow |

Arkon Vault was not found in the public Gemini extension gallery during the
July 30 recheck. The gallery is no longer treated as a pending launch gate
because Google now directs individual terminal users to Antigravity CLI.
Arkon Vault remains available through the production Streamable HTTP endpoint
and the public connector repository; no Google gallery publication is claimed.
Evidence: `https://github.com/google-gemini/gemini-cli/discussions/28017`.

## Verified registry record

- Name: `io.github.Havix0101/arkon-vault`
- Title: `Arkon Vault`
- Version: `1.6.0`
- Status: `active`
- Transport: `streamable-http`
- Endpoint: `https://vault.arkoncybersecurity.com/mcp`
- Published: `2026-07-27T23:05:29Z`

## Commercial and licensing boundary

The public repository licenses only connector metadata and workflow guidance under MIT. It does not publish or license the proprietary Arkon Vault application or hosted backend.

The official MCP Registry dedicates submitted registry metadata to the public domain under its registry terms. That affects the public listing metadata, not the application source or hosted service.
