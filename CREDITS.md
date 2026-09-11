# Credits

The rule set began as two tables in an internal design-intelligence project that had
ingested and analysed roughly 2,600 Awwwards Site-of-the-Day winners:

- `banned_patterns` — 10 rules describing what to reject
- `sacred_patterns` — 9 rules describing what order to work in

That project was retired. Measuring it before shutdown was instructive and worth recording:

- Its LLM-generated design specs averaged **19.7 "not found in CSS"** entries each;
  about **73%** were too weak to use.
- About **38%** of its stored reference screenshots were blank frames, preloaders,
  cookie walls, or captures of domains that had since expired.

The rules survived the project that produced them. That is the whole point of writing
guardrails down separately from the machinery that generated them.

Sections A–D and the measurable tests were then rewritten against real rejections on a
working client project, which is where rules 2, 4 and 10 come from — each one is a
specific thing a client pointed at and said "this looks cheap".
