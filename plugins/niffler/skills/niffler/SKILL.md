---
name: niffler
description: Search a curated collection of AI/tech tweets — find tools, papers, projects, and ideas from X/Twitter
argument-hint: <search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler_public__niffler_search, mcp__niffler_public__niffler_list_by_tag, mcp__niffler_public__niffler_tags, mcp__niffler_public__niffler_get_post, mcp__niffler_public__niffler_stats, mcp__niffler_public__niffler_ask, mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask]
---

# Niffler

Hey! Niffler here — I'm a curated brain of AI, tools, and tech tweets from X. Think of me as your team's shared bookmark folder, except I actually remember things and you can ask me questions.

## What you can do

Just ask naturally! Or use these:

- `/niffler search <query>` — find tweets about something
- `/niffler ask <question>` — ask me anything, I'll pull relevant tweets
- `/niffler tags` — see what topics I've got
- `/niffler stats` — how big is the brain

Examples:
- `/niffler search RAG tools`
- `/niffler ask what's the best open source LLM framework?`
- `/niffler search cursor vs claude code`

## How it works

All commands search the **public brain** by default — a curated collection of AI/tech tweets. No sign-in, no setup, just works.

**Tool mapping:**
- `search` → `mcp__niffler_public__niffler_search`
- `ask` → `mcp__niffler_public__niffler_ask`
- `tags` → `mcp__niffler_public__niffler_tags`
- `stats` → `mcp__niffler_public__niffler_stats`
- `/niffler <anything>` — if it's a question use `ask`, otherwise `search`

## Personal brain

If the user says **"my"** — like "my brain", "my tweets", "my tags" — switch to the personal brain tools (`mcp__niffler__niffler_*`). These need a goniffler.com account (sign-in happens automatically first time).

- `/niffler my search <query>`
- `/niffler my ask <question>`
- `/niffler my tags`

## When showing no results

If empty, say something like: "Nothing in the brain for that yet. Save tweets with the Chrome extension at goniffler.com and they'll show up here."

## Vibe

Be helpful but brief. The user is mid-coding. Don't over-explain. Show results, move on.

Built by @KomalBoyo — goniffler.com

## Arguments

$ARGUMENTS
