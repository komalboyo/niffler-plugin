# Niffler — Claude Code Plugin

Search your personal X/Twitter knowledge graph and the public brain — right from Claude Code.

## Install

```
/plugin marketplace add komalboyo/niffler-plugin
/plugin install niffler
```

## Two Brains

This plugin gives you access to two brains:

### Your Personal Brain
Your own saved tweets. First time you use it, your browser opens to sign in at [goniffler.com](https://goniffler.com) — after that it stays connected.

Save tweets using the [Chrome extension](https://goniffler.com) or at goniffler.com. Then query them here:

```
/niffler search transformer architecture
/niffler ask what tools were recommended for RAG?
/niffler tags
/niffler stats
```

### The Public Brain
A curated collection of AI/tech tweets. No sign-in needed — works immediately:

```
/niffler public search open source LLM tools
/niffler public ask what's the best framework for agents?
/niffler public tags
```

## How It Works

1. **Install the plugin** (two commands above)
2. **Save tweets** via the Chrome extension or goniffler.com — AI auto-tags them
3. **Query from Claude Code** — search, ask questions, browse by tags
4. New tweets you save are instantly available here — no sync needed

## Tools

**Personal brain** (`/niffler`):
- `niffler_search` — full-text search your saved tweets
- `niffler_ask` — ask questions, get answers from your content
- `niffler_list_by_tag` — browse by tag
- `niffler_tags` — see all your tags
- `niffler_get_post` — full post details
- `niffler_stats` — brain overview

**Public brain** (`/niffler public`):
- Same tools, prefixed with `niffler-public`

## Links

- [goniffler.com](https://goniffler.com) — hosted version + Chrome extension
- [Open source](https://github.com/komalboyo/niffler-opensource) — self-host your own instance
