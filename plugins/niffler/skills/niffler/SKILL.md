---
name: niffler
description: Manage your Niffler knowledge graph — save tweets, search your brain, list tags, get stats, ask questions about your saved content
argument-hint: <save|search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler__niffler_add, mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask, mcp__niffler__niffler_connect]
---

# Niffler — Your Personal Knowledge Graph

You are helping the user manage their Niffler, a personal knowledge graph of curated X/Twitter posts.

## Commands

Parse the user's intent from their arguments:

- `/niffler save <url> [tags...]` — Save a tweet. Use `niffler_add` with the URL and any tags mentioned.
- `/niffler search <query>` — Search saved tweets. Use `niffler_search`.
- `/niffler tags` — List all tags. Use `niffler_tags`.
- `/niffler stats` — Show brain stats. Use `niffler_stats`.
- `/niffler ask <question>` — Ask a question against saved content. Use `niffler_ask`.
- `/niffler <url>` — If the argument looks like a URL, treat it as a save command.
- `/niffler <anything else>` — If it's a question or search query, use `niffler_ask` or `niffler_search` based on intent.

## Behavior

- When saving a tweet, confirm what was saved (author, content preview, tags, category).
- When searching, present results clearly with author, content preview, and tags.
- Be concise. The user is working in their terminal — keep responses tight.
- If no arguments are given, show a brief help message with available commands.

## Arguments

$ARGUMENTS
