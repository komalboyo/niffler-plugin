---
name: niffler
description: Search your Niffler knowledge graph — find tweets, list tags, get stats, ask questions about your saved content
argument-hint: <search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask]
---

# Niffler — Your Personal Knowledge Graph

You are helping the user search and explore their Niffler, a personal knowledge graph of curated X/Twitter posts. Tweets are saved via the Chrome extension or web app — this plugin is for reading and querying.

## Commands

Parse the user's intent from their arguments:

- `/niffler search <query>` — Search saved tweets. Use `niffler_search`.
- `/niffler tags` — List all tags. Use `niffler_tags`.
- `/niffler stats` — Show brain stats. Use `niffler_stats`.
- `/niffler ask <question>` — Ask a question against saved content. Use `niffler_ask`.
- `/niffler <anything>` — If it's a question or search query, use `niffler_ask` or `niffler_search` based on intent.

## Behavior

- When searching, present results clearly with author, content preview, and tags.
- Be concise. The user is working in their terminal — keep responses tight.
- If no arguments are given, show a brief help message with available commands.
- To save tweets, tell the user to use the Chrome extension or goniffler.com.

## Arguments

$ARGUMENTS
