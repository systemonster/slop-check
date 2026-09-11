# slop-check

A ship-gate checklist that catches AI-generated design slop before you call a page done.

Twelve questions in four groups, plus four rules about the **order** you work in. One "yes" means the page is not finished.

**→ [Read the checklist](https://systemonster.github.io/slop-check/)**

---

## Why this exists

A design can be technically fine — accessible, responsive, on-brand — and still read as machine-made. That failure has a small number of repeatable causes, and once they are written down they are easy to catch.

The rule set started as two tables in a design-intelligence project that had ingested about 2,600 Awwwards Site-of-the-Day winners. That project was retired; measuring it before shutdown was itself instructive (73% of its generated design specs were too weak to use, 38% of its reference screenshots were blank frames or cookie walls). **The rules outlived the machinery that produced them.** See [CREDITS.md](CREDITS.md).

Sections A–D were then rewritten against real client rejections — each of rules 2, 4 and 10 is a specific thing someone pointed at and called cheap.

## Install

As a [Claude Code](https://claude.com/claude-code) skill:

```bash
npx skills add systemonster/slop-check
```

Or copy `SKILL.md` into `.claude/skills/slop-check/` in your project, or `~/.claude/skills/` to have it everywhere.

It also works as a plain checklist for humans — nothing about it is tool-specific.

## The short version

**Work in this order.** Typography before decoration · layout from the content's logic, not a card grid · spacing rhythmic and uneven · motion with a doctrine.

**Then check:** template hero · stock-photo hero · three equal cards · same skeleton different paint · the purple-gradient-plus-Inter trio · gradient CTA · neutral sans everywhere · SaaS drift · ornamental scroll · hover that only changes `background-color` · style without evidence · fabricated proof.

**Then measure:** describe each page's mobile first screen in six words — if two pages get the same six words, it is a template. Desaturate the thumbnails — can you still tell them apart?

## Contributing

Rules earn their place by catching something real. If you open a PR adding one, say what it caught — a page, a review, a rejection. Rules without a story get closed.

## License

MIT — see [LICENSE](LICENSE).

Built by [lovefengis](https://lovefengis.com), a web and software studio in İzmir, Türkiye.
