---
name: niffler
description: Search a curated collection of AI/tech tweets — find tools, papers, projects, and ideas from X/Twitter
argument-hint: <search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler_public__niffler_search, mcp__niffler_public__niffler_list_by_tag, mcp__niffler_public__niffler_tags, mcp__niffler_public__niffler_get_post, mcp__niffler_public__niffler_stats, mcp__niffler_public__niffler_ask, mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask]
---

# Niffler — AI/Tech Tweet Search

Search a curated collection of AI, tools, and tech tweets from X/Twitter. No sign-in needed — works immediately.

## Commands

- `/niffler search <query>` — Search tweets. Use `mcp__niffler_public__niffler_search`.
- `/niffler ask <question>` — Ask a question, get answers from saved tweets. Use `mcp__niffler_public__niffler_ask`.
- `/niffler tags` — List all tags. Use `mcp__niffler_public__niffler_tags`.
- `/niffler stats` — Brain overview. Use `mcp__niffler_public__niffler_stats`.
- `/niffler <anything>` — If it's a question use `niffler_ask`, otherwise `niffler_search`.

All commands above use the **public brain** by default.

## Personal Brain

If the user says "my brain", "my tweets", "personal", or "mine" — use the personal brain tools (`mcp__niffler__niffler_*`) instead. These require sign-in (happens automatically on first use).

- `/niffler my search <query>` — Search personal brain.
- `/niffler my tags` — Personal tags.
- `/niffler my ask <question>` — Ask against personal brain.

## Behavior

- **Default to the public brain** — no sign-in friction, works for everyone.
- Present results clearly with author, content preview, and tags.
- Be concise. The user is working in their terminal.
- To save tweets to a personal brain, tell the user to sign up at goniffler.com and install the Chrome extension.

## Arguments

$ARGUMENTS
