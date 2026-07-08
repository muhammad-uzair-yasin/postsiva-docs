# Postsiva Docs — Site Map

**Status (2026-07-08):** ~66 MDX pages after audit fixes (paths, nav dedupe, accuracy).

Config: `docs.json` (Mintlify). Index: `llms.txt`.

## Pages

### Get started
- introduction, quickstart, authentication, workspaces, guides/complete-setup

### Features
- overview, publishing, scheduling-and-drafts, inbox, analytics
- ai-content, ai-watcher, personas, agents, workspaces-and-team, clients, ads

### REST API
- overview, posting, posting-parameters, posts, scheduled-posts, drafts
- analytics, comments, oauth, user-profiles, media
- ai-content, ai-watcher, agent-chat, gpt-actions

### MCP
- overview, connect, tools, cursor, n8n, chatgpt

### Platforms
- overview + LinkedIn, Facebook, Instagram, TikTok, YouTube, Threads, Pinterest, Bluesky
- snapchat, whatsapp

### Guides
- media-guidelines, character-limits, scheduling, drafts

### Integrations
- overview, n8n, zapier, make, curl, claude, chrome-extension, whatsapp

### Errors & reference
- errors/*, reference/plans, reference/ids-and-scopes

## Canonical paths (quick reference)

| Area | Path |
|------|------|
| Posting | `/unified/post/*` |
| OAuth | `/unified/oauth/*` |
| Media | `/media/*` |
| Profiles | `/unified/user-profiles/` |
| Legacy (temp) | `/social/*` → rewritten to `/unified/*` |

## Preview
```bash
cd postsiva-docs && npm run dev
# Node 22 via /usr/bin — see README
```

## Follow-ups (optional)
- Embed OpenAPI / Postman collection
- Billing API page (`GET /billing/plans`)
- Persona builder REST per platform
