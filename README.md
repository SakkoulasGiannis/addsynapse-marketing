# Google Analytics, Search Console & Google Ads for Claude or ChatGPT (AddSynapse skill + MCP)

**Ask why your traffic dropped. Get an answer you understand.** Claude or ChatGPT read your Google Analytics 4, Google Search Console and Google Ads and answer in three parts: what happened, why, and what to do, with the numbers from your own accounts. **Read-only:** nothing can be changed in Google.

Free forever · 100 actions a day, Google Analytics and Search Console included. Google Ads: first week free, then Pro €9 a month. → https://addsynapse.com/analytics

## Install the skill
| Where | How |
|---|---|
| **Claude Code** | `/plugin marketplace add SakkoulasGiannis/addsynapse-marketing` then `/plugin install addsynapse-marketing@addsynapse-marketing`. Adds the skill and both connectors (MCP) in one step. |
| **Claude** (web/desktop) | [Download the zip](https://github.com/SakkoulasGiannis/addsynapse-marketing/releases/latest/download/addsynapse-marketing.zip) → Settings → Skills → Upload skill. |
| **Other agents** (Cursor, Codex, …) | Copy [`skills/addsynapse-marketing`](skills/addsynapse-marketing/SKILL.md) into your agent's skills folder and add the MCP servers below. |

## Connect
1. **Add the connectors** (custom connector in Claude: Settings → Connectors → Add custom connector; ChatGPT, any plan: Plugins → + → Add custom MCP server):
   - AddSynapse Analytics (GA4 + Search Console): `https://api.addsynapse.com/mcp/analytics`
   - Ads Manager for Google Ads & Meta (Google Ads): `https://api.addsynapse.com/mcp/ads`
2. **Sign up → Allow** (free AddSynapse account).
3. **Connect Google** with one click from the link the AI gives you (read-only access).

## Try
- "Using AddSynapse, why did my traffic drop last week?"
- "Using AddSynapse, which landing pages get visits but no sales?"
- "Using AddSynapse, which Google searches show my site but get few clicks?"
- "Using AddSynapse, which search terms cost me money without conversions?"

## What it reads
- **Google Analytics 4:** period comparisons, landing pages, custom reports.
- **Search Console:** lost clicks and positions, low-CTR queries, opportunities for one page.
- **Google Ads:** campaigns and cost, trend vs previous period, wasted spend, conversion actions.
- **Meta (Facebook & Instagram) ads:** coming soon.

## Known limitations
- Read-only: it does not change campaigns, budgets or settings.
- Meta ads are not available yet.
- Google Analytics 4 only.

This repository holds the public skill and docs. The service is run by [AddSynapse](https://addsynapse.com).
