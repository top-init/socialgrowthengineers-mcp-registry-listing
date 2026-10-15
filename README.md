# socialgrowthengineers-mcp-registry-listing

## At a glance

| | |
|---|---|
| **What it is** | Config only: the MCP Registry entry (`server.json`, published as `com.socialgrowthengineers/mcp`) and a client config (`.mcp.json`). No server code. |
| **Where it runs** | The MCP server lives in `top-init/socialgrowthengineers.com` (`pages/api/mcp`), served at `https://www.socialgrowthengineers.com/mcp`. |
| **How it deploys** | Automatic. Bump `version` in `server.json` and merge to `main` → the `publish` workflow republishes to the MCP Registry. The same version cannot be published twice. |
| **Auth for publishing** | DNS domain proof: the apex TXT record `v=MCPv1; k=ed25519; p=<public key>` (Cloudflare); the private key (hex) is the `MCP_REGISTRY_PRIVATE_KEY` secret on the `mcp-registry-publish` environment, which needs a reviewer to approve each run. |
| **How to check it's healthy** | `curl -s "https://registry.modelcontextprotocol.io/v0/servers?search=socialgrowthengineers"` shows the listing. |

## Social Growth Engineers MCP server

A hosted remote MCP server for short-form marketing research: viral TikTok and Reels videos, hooks, app growth playbooks, articles and reports, plus live App Store data.

- **Endpoint:** `https://www.socialgrowthengineers.com/mcp`
- **Transport:** Streamable HTTP
- **Auth:** OAuth 2.1. Your MCP client discovers it on first connect and opens a sign-in.
- **Website:** https://www.socialgrowthengineers.com

## Connect

Claude Code:

```bash
claude mcp add --transport http socialgrowthengineers https://www.socialgrowthengineers.com/mcp
```

Any other client: use the entry in `.mcp.json`.

## License

The files in this repo are MIT licensed. Use of the hosted service follows the terms at https://www.socialgrowthengineers.com.
