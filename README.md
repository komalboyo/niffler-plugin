# Niffler — Claude Code Plugin

Save and search X/Twitter posts from Claude Code. Build a personal AI knowledge graph with auto-categorization, tagging, and full-text search.

## Install

```
/plugin marketplace add komalboyo/niffler-plugin
/plugin install niffler
```

On first use, your browser will open to sign in at [goniffler.com](https://goniffler.com). After that, it just works.

## Usage

```
/niffler save https://x.com/karpathy/status/123456
/niffler search "transformer architecture"
/niffler tags
/niffler stats
/niffler ask "what tools were recommended for RAG?"
```

The MCP tools are also available directly — Claude will use them when relevant to your conversation.

## What you get

- **niffler_add** — Save a tweet (scrapes content, auto-categorizes with AI)
- **niffler_search** — Full-text search across your saved tweets
- **niffler_list_by_tag** — Browse by tag
- **niffler_tags** — See all your tags
- **niffler_get_post** — Get full post details
- **niffler_stats** — Brain overview
- **niffler_ask** — Ask questions, get answers from your saved content
- **niffler_connect** — Link related posts

## Self-host

Niffler is open source. Run your own instance: [github.com/komalboyo/niffler](https://github.com/komalboyo/niffler)
