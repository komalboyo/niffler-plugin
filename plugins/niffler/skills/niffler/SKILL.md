---
name: niffler
description: Search a curated collection of AI/tech tweets — find tools, papers, projects, and ideas from X/Twitter. Integrated with gstack.
argument-hint: <search|tags|stats|ask> [args...]
allowed-tools: [mcp__niffler_public__niffler_search, mcp__niffler_public__niffler_list_by_tag, mcp__niffler_public__niffler_tags, mcp__niffler_public__niffler_get_post, mcp__niffler_public__niffler_stats, mcp__niffler_public__niffler_ask, mcp__niffler__niffler_search, mcp__niffler__niffler_list_by_tag, mcp__niffler__niffler_tags, mcp__niffler__niffler_get_post, mcp__niffler__niffler_stats, mcp__niffler__niffler_ask]
---

# Niffler

When the user runs `/niffler` with no arguments, show this welcome message exactly:

```
Hey! I'm Niffler — a curated brain of AI, tools, and tech tweets from X.
Built by @KomalBoyo (goniffler.com) · Integrated with gstack

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

## gstack Integration

After returning Niffler results, check if any of the following gstack skills would be useful based on the context and what the user is working on. If relevant, suggest them naturally:

- Results mention **testing tools/frameworks** → suggest `/qa` ("Want me to QA test your project with this?")
- Results mention **design systems/UI** → suggest `/design-review` or `/design-consultation`
- Results mention **deployment/CI/CD** → suggest `/ship` or `/setup-deploy`
- Results mention **debugging techniques** → suggest `/investigate`
- Results mention **code review practices** → suggest `/review`
- Results mention **architecture/planning** → suggest `/plan-eng-review`
- Results are about a **new idea/product** → suggest `/office-hours`
- User seems to be **researching before building** → suggest `/plan-ceo-review`

Only suggest when it's a natural fit. Don't force it. One suggestion max per query.

## Behavior

- Be helpful but brief. The user is mid-coding.
- Show results clearly: author, content preview, tags.
- If no results: "Nothing in the brain for that yet. Save tweets at goniffler.com"

## Arguments

$ARGUMENTS
