---
name: steiner-research
description: Use when the user asks what Rudolf Steiner said, wrote or taught about a topic, wants a Steiner quote or source, or asks about anthroposophy, biodynamic agriculture, Waldorf education or anthroposophic medicine in Steiner's own words. Finds and cites passages from the Gesamtausgabe through the steiner MCP server.
---

# Researching Rudolf Steiner's own words

The `steiner` MCP server holds the German full text of Steiner's collected works (Gesamtausgabe, GA).

## Searching

- Search in German, whatever language the user writes in. Translate the user's topic into the German terms Steiner used: soil fertility → Bodenfruchtbarkeit, Dünger; etheric body → Ätherleib; threefold social order → Dreigliederung des sozialen Organismus.
- The index stems German words, so Düngung also finds Dünger. Older spellings are not normalised: try daß, Entwickelung, Thätigkeit, Theil where modern spelling fails.
- Start broad, then narrow with more words, a quoted phrase, a volume (`ga`) or a date range.
- When a hit looks relevant, read the surrounding passages with `read` before quoting, so the quote is not taken out of context.
- To answer "when" or "how often" questions, use `count_matches` grouped by year, volume or place.

## Answering

- Quote only text that appears in the tool results, in the original German, and add a translation when the user writes in another language. Mark translations as such.
- Cite every quote as: GA number, page(s), and for lectures the place and date, e.g. *GA 327, p. 101 (Koberwitz, 12 June 1924)*.
- Distinguish what Steiner said from interpretation, including your own.
- If the database has no full text for a volume, say so rather than quoting from memory.
- The texts are older editions from steiner.wiki (CC BY-NC-SA 4.0). Mention the source when quoting at length.
