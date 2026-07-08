# Postsiva Developer Docs

Developer documentation for the Postsiva REST API, workspace API keys, and Unified MCP server.

Modeled after [Ayrshare docs](https://www.ayrshare.com/docs/introduction) structure: introduction → quickstart → API reference by domain → MCP → platform guides → integrations.

## Local dev

Mintlify requires **Node 20.17–24** (not 25+). Your default shell may use Homebrew Node 26.

You have **`n`** installed (`/usr/local/bin/n`). Switch globally:

```bash
sudo n 22.22.0
node -v   # v22.x
```

Or only for docs (npm scripts already prepend `/usr/bin`):

```bash
cd postsiva-docs
npm install
npm run dev
```

Open http://localhost:3000 (or 3001 if 3000 is busy).

## Deploy

Host on [Mintlify](https://mintlify.com) (recommended, same stack as Ayrshare) or export static if needed.

Suggested production URL: `https://docs.postsiva.com`

## Content sources (backend)

When writing or updating pages, sync from:

| Source | Use for |
|--------|---------|
| `postsiva-backend/app/modules/*/curl.json` | REST endpoint examples |
| `postsiva-backend/app/modules/openai_agents/whatsapp_agents/tools/` | MCP tool behavior |
| MCP tool descriptors in Cursor (`user-Postsiva` MCP) | Tool names + parameters |
| `postsiva-backend/app/modules/workspace_api_keys/` | API key scopes |
| `postsiva-backend/app/modules/unified_mcp/` | MCP auth + server |

## AI index

`llms.txt` at repo root — machine-readable page index (like Ayrshare's `llms.txt`).
