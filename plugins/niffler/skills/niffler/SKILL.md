---
name: niffler
description: Search a curated collection of AI/tech tweets — find tools, papers, projects, and ideas from X/Twitter
argument-hint: <search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler_public__niffler_search, mcp__niffler_public__niffler_list_by_tag, mcp__niffler_public__niffler_tags, mcp__niffler_public__niffler_get_post, mcp__niffler_public__niffler_stats, mcp__niffler_public__niffler_ask, mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask]
---

# Niffler

When the user runs `/niffler` with no arguments, show this welcome message exactly:

```
Hey! I'm Niffler — a curated brain of AI, tools, and tech tweets from X.
Built by @KomalBoyo (goniffler.com)

SEARCH THE PUBLIC BRAIN (works instantly, no sign-in):
  /niffler search <query>     — find tweets about something
  /niffler ask <question>     — ask me anything, I'll pull relevant tweets
  /niffler tags               — see what topics I've got
  /niffler stats              — how big is the brain

SEARCH YOUR PERSONAL BRAIN (needs a goniffler.com account):
  /niffler my search <query>  — search your own saved tweets
  /niffler my ask <question>  — ask against your saved tweets
  /niffler my tags            — your tags

Save tweets with the Chrome extension at goniffler.com.
Your personal brain updates in real-time.

Try: /niffler search AI agents
```

## How it works

All commands search the **public brain** by default — no sign-in, no setup.

**Tool mapping:**
- `search` → `mcp__niffler_public__niffler_search`
- `ask` → `mcp__niffler_public__niffler_ask`
- `tags` → `mcp__niffler_public__niffler_tags`
- `stats` → `mcp__niffler_public__niffler_stats`
- `/niffler <anything>` — if it's a question use `ask`, otherwise `search`

## Personal brain

If the user says **"my"** — like "my brain", "my search", "my tags" — switch to personal brain tools (`mcp__niffler__niffler_*`). Sign-in happens automatically first time.

## Behavior

- Be helpful but brief. The user is mid-coding.
- Show results clearly: author, content preview, tags.
- If no results: "Nothing in the brain for that yet. Save tweets at goniffler.com"

## Arguments

$ARGUMENTS
