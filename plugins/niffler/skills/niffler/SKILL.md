---
name: niffler
description: Search your Niffler knowledge graph or the public brain — find tweets, list tags, get stats, ask questions
argument-hint: <search|tags|stats|ask|public> [args...]
allowed-tools: [mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask, mcp__niffler_public__niffler_search, mcp__niffler_public__niffler_list_by_tag, mcp__niffler_public__niffler_tags, mcp__niffler_public__niffler_get_post, mcp__niffler_public__niffler_stats, mcp__niffler_public__niffler_ask]
---

# Niffler — Knowledge Graph for X/Twitter

You are helping the user search and explore Niffler brains. There are two brains available:

- **Personal brain** (`niffler` tools) — the user's own saved tweets. Requires sign-in (happens automatically on first use).
- **Public brain** (`niffler-public` tools) — a curated collection of AI/tech tweets. No sign-in needed.

## Commands

Parse the user's intent from their arguments:

- `/niffler search <query>` — Search personal brain. Use `mcp__niffler__niffler_search`.
- `/niffler tags` — List personal tags. Use `mcp__niffler__niffler_tags`.
- `/niffler stats` — Personal brain stats. Use `mcp__niffler__niffler_stats`.
- `/niffler ask <question>` — Ask against personal brain. Use `mcp__niffler__niffler_ask`.
- `/niffler public search <query>` — Search the public brain. Use `mcp__niffler_public__niffler_search`.
- `/niffler public tags` — Public brain tags. Use `mcp__niffler_public__niffler_tags`.
- `/niffler public ask <question>` — Ask against the public brain. Use `mcp__niffler_public__niffler_ask`.
- `/niffler <anything>` — Default to personal brain. If it's a question, use `niffler_ask`; otherwise `niffler_search`.

## Behavior

- Default to **personal brain** unless the user says "public" or "public brain".
- Present results clearly with author, content preview, and tags.
- Be concise. The user is working in their terminal.
- If no arguments are given, show available commands for both brains.
- To save tweets, tell the user to use the Chrome extension or goniffler.com.

## Arguments

$ARGUMENTS
