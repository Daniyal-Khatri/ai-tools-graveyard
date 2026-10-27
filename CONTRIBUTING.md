# Contributing to AI Tools Graveyard

Thank you for helping keep the record accurate. This list only works if every
grave is real, so the rules are strict — but simple.

## The one rule that matters

**No source, no tombstone.** Every tool added here must have a public source
that proves it died: the company's own shutdown announcement, a reputable news
article, or the product's official page stating it was discontinued.

Blog posts repeating a rumor do not count. "I heard it shut down" does not
count. If you cannot link to proof, do not open the PR.

## How to add a dead tool

1. Add the tool to `data/dead-tools.json`. That file is the single source of
   truth — the README tables and the CSV are built from it.
2. Use exactly these fields:

```json
{
  "name": "Tool Name",
  "category": "Chatbot",
  "description": "One short line saying what the tool did, in easy words.",
  "born": "2021",
  "died": "December 31, 2025",
  "raised": "$21M",
  "cause": "Shutdown — one short line on what happened.",
  "source_url": "https://link-to-the-proof",
  "survived_by": "Name of a free or freemium alternative that is still alive"
}
```

3. Categories: `Chatbot`, `Image`, `Video`, `Voice & Audio`, `Writing`,
   `Presentations`, `Website Builder`, `Search`, `Productivity`, `Other`.
4. The `survived_by` tool must be alive and free or freemium **today**. If the
   alternative also died, pick another one — or note both deaths.
5. One tool per pull request. Say in the PR where your source comes from.
6. `born` is the year the product launched (or the company was founded).
   `raised` is the total funding, in a short form like `"$450M"`. Both need a
   real source too — if you cannot source one, leave it as `""`. A blank is
   honest; a guessed number gets the PR closed.

## Not dead yet?

If a tool has announced a shutdown date in the future, or is in serious
trouble (bankruptcy, acquisition wind-down) but **still works today**, it
belongs in the README's "Intensive Care" section, not the graveyard. When it
actually closes, move it into the data with its real death date and source.

## Reporting a mistake

Wrong date? Wrong cause? A tool we buried that is actually alive? Open an
issue with a source link. Accuracy beats size — a wrong grave gets fixed or
removed, fast.

## Style

- Easy words. Short lines. A beginner should understand every entry.
- No marketing language, no hype, no jokes at the expense of the people who
  lost money or work when a tool died. The graveyard is respectful; the facts
  are interesting enough on their own.
