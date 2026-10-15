# Social Growth Engineers MCP server

**[Social Growth Engineers](https://www.socialgrowthengineers.com/?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing)** (SGE) gives your AI assistant the research behind short-form growth: viral TikTok and Reels videos, the hooks that made them work, app growth playbooks, articles and reports, plus live App Store data.

[Website](https://www.socialgrowthengineers.com/?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing) · [Join SGE](https://www.socialgrowthengineers.com/join?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing) · [Prometheus research agent](https://www.socialgrowthengineers.com/prometheus?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing) · [Official MCP Registry](https://registry.modelcontextprotocol.io/v0/servers?search=com.socialgrowthengineers)

| | |
|---|---|
| **Endpoint** | `https://www.socialgrowthengineers.com/mcp` |
| **Transport** | Streamable HTTP (remote, hosted, nothing to install) |
| **Auth** | OAuth 2.1. Your client opens an SGE sign-in on first connect. No API key to copy. |
| **Access** | Included with an [SGE membership](https://www.socialgrowthengineers.com/join?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing) |
| **Registry name** | `com.socialgrowthengineers/mcp` |

## What you can ask

- "Show me the most viral TikToks for meditation apps this month and the hooks they used."
- "Which hook formats are working best for fitness apps right now?"
- "Break down the growth strategy behind Cal AI."
- "Find SGE articles on UGC creator programs for apps."
- "Analyze this TikTok: what made it go viral?"

## Tools

| Area | Tools |
|---|---|
| Viral videos | Search viral short-form videos, find similar videos, analyze a video, content analytics |
| Hooks | Hook intelligence: which openings and formats perform, by vertical |
| Apps | Search and list apps, app accounts, app growth strategy, similar apps, categories |
| Articles & reports | Search and read SGE articles, similar articles, generate reports |
| App Store data | Live rankings and app details via [App Store Tracker](https://www.appstoretracker.com/?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing) |

## Connect

**Claude Code**

```bash
claude mcp add --transport http socialgrowthengineers https://www.socialgrowthengineers.com/mcp
```

**Any MCP client** (Claude Desktop, Cursor, Windsurf, VS Code…): add the URL as a remote MCP server, or use [`.mcp.json`](.mcp.json). Sign in when prompted.

```json
{
  "mcpServers": {
    "socialgrowthengineers": {
      "type": "http",
      "url": "https://www.socialgrowthengineers.com/mcp"
    }
  }
}
```

## Find it in MCP directories

- [Official MCP Registry](https://registry.modelcontextprotocol.io/v0/servers?search=com.socialgrowthengineers)
- [Smithery](https://smithery.ai/server/topinit/socialgrowthengineers)
- [MCP.so](https://mcp.so/servers/social-growth-engineers)
- [AllMCPs](https://allmcps.com/mcp/social-growth-engineers)
- [MCP Repository](https://mcprepository.com/top-init/socialgrowthengineers-mcp-registry-listing)

## Also from the same team

- [App Store Tracker MCP](https://github.com/top-init/appstoretracker-mcp-registry-listing): iOS rankings, reviews, keywords and revenue estimates
- [Shortimize MCP](https://github.com/top-init/shortimize-mcp-registry-listing): TikTok, Reels and Shorts analytics

## About this repo

| | |
|---|---|
| **What it is** | Config only: the MCP Registry entry (`server.json`) and a client config (`.mcp.json`). The server itself runs at the endpoint above. |
| **How it deploys** | Bump `version` in `server.json` and merge to `main`. The `publish` workflow republishes to the MCP Registry after a maintainer approves the run. |
| **Ownership proof** | DNS TXT record on socialgrowthengineers.com. The signing key is a GitHub environment secret. |
| **Health check** | `curl -s "https://registry.modelcontextprotocol.io/v0/servers?search=socialgrowthengineers"` |

The files in this repo are MIT licensed. Use of the hosted service follows the terms at [socialgrowthengineers.com](https://www.socialgrowthengineers.com/?utm_source=github&utm_medium=referral&utm_campaign=mcp-listing).
