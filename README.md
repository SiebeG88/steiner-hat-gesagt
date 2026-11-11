# Was hat Steiner gesagt? – Claude plugin

What did Steiner say? This plugin connects Claude to a full-text database of Rudolf Steiner's collected works (Gesamtausgabe, GA) so that Claude can find, read and quote what Steiner actually said or wrote, with GA number, page and lecture date for every quote.

## What it contains

- **MCP connector** `steiner`: a remote, read-only server at `https://was-hat-steiner-gesagt.vercel.app/mcp`. It needs no account or key.
- **Skill** `steiner-research`: guidance for Claude on searching in German, reading context before quoting, and citing correctly.

The connector offers five read-only tools: `search` (German full-text search with stemming, filters for volume and lecture date), `read` (a chapter, page range or the text around a hit), `list_works` (the catalogue of all 383 volumes), `get_work` (one volume's table of contents) and `count_matches` (how often a topic occurs by year, volume or place).

## Data and privacy

The plugin runs no local code. The only network traffic is the tool calls Claude makes to the connector above: the search words or volume numbers Claude chooses. The service has no accounts, cookies or analytics and does not store search words. Full privacy policy: https://was-hat-steiner-gesagt.vercel.app/#privacy

## Source

The database holds 307 volumes of full text (about 190,000 passages) from [steiner.wiki](https://steiner.wiki), which republishes the material of the former Freie Verwaltung des Nachlasses Rudolf Steiners. These are older editions. Steiner's own texts are in the public domain; the wiki's editorial work is licensed CC BY-NC-SA 4.0, so the service is free and non-commercial.

## Try asking

- What did Steiner say about the cow horn preparations in the Agriculture Course?
- In which years did Steiner speak most about the threefold social order?
- Show me the table of contents of GA 293 and summarise the first lecture.

Plugin licence: MIT.
