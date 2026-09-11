---
name: slop-check
description: Ship-gate checklist that catches AI-generated design slop before you call a page done. Use when building or reviewing a landing page, hero, card, button or section; when a design "looks basic" and you can't say why; or right after a design gets rejected.
---

# Slop check

A design that is *technically fine* and still reads as machine-made fails for a small number of repeatable reasons. This is the list of them.

Run it before you call anything done. **One "yes" means the page is not finished.**

Provenance: distilled from the banned-pattern and sacred-pattern rules of an abandoned design-intelligence project that had ingested ~2,600 Awwwards Site-of-the-Day winners, plus lessons from real client rejections. See CREDITS.

---

## Order matters — do these first

Skipping a step here comes back later as slop you can't name.

1. **Typography before decoration.** Establish hierarchy — heading/body/label scale, weight contrast, line length — before you touch color, shadow or radius. A page decorated on top of flat hierarchy cannot be rescued by styling.
2. **Layout comes from the content's logic, not from a card grid.** If "card grid" was the reflex answer, the layout was not designed. Ask what shape the content actually is.
3. **Spacing should be rhythmic and uneven.** Giving every section the same vertical padding is the quietest source of template-feel. Build a rhythm: places that breathe, places that compress.
4. **Motion needs a doctrine.** Motion must express hierarchy, time, or spatial logic. "It looks nice" does not pass. If removing an animation costs the reader nothing, remove it.

---

## A. Composition — most failures are here

1. **Template hero?** Hero → features → pricing, assembled by default rather than because the content asked for it.
2. **Stock-photo hero?** Photo + headline overlaid + two buttons. This is the pattern even when the photo is real and good. Either the image *is* the hero, or there is no hero image.
3. **Three equal cards?** An equal-width three-card grid used as the reflex answer to "explain the benefits". Fine when the content is genuinely three peers; never as a default.
4. **Same skeleton, different paint?** Put it beside the previous page. If the only differences are color and border-radius, it is the same page twice. What must differ: **hero media type, the interactive module, the typeface pairing.**

## B. Material

5. **The default AI trio?** Purple/indigo gradient + Inter or Roboto as primary + uniform "safe" rounding. Present together, the page reads as generated no matter how well it is executed.
6. **Gradient CTA?** A purple/indigo gradient button used as the default accent move.
7. **Neutral sans everywhere?** All type flattened into quiet sans weights with no hierarchy and no voice.
8. **SaaS drift?** Generic SaaS polish applied when the brief called for editorial, cultural, luxury or sector work. A hair salon's site should not look like Stripe.

## C. Motion and interaction

9. **Ornamental scroll?** Scroll-linked motion that does not change comprehension, pacing, or the meaning of a section. Cut it.
10. **Unfinished interactive element?** If only `background-color` changes on hover, the element is not finished. **At least three things should move together — surface, position, and shadow** — and the shadow should be a softened version of the element's own color, not neutral black.

## D. Evidence and honesty

11. **Style without evidence?** "I think it looks better" is not evidence. Cite a measured reference value, a spec, or data. If you are claiming a reference does something, **measure it** with `getComputedStyle` — do not eyeball it.
12. **Fabricated proof?** Testimonials, star ratings, client logos, "N happy customers", award badges, suspiciously precise percentages. If there is no source, remove it — including on demo and concept pages.

---

## Measurable tests (when there is more than one page)

- **Skeleton test** — describe each page's mobile first screen in six words. If two pages get the same six words, it is a template.
- **Greyscale blind test** — desaturate the thumbnails. Can you still tell them apart? This is where "changed the colors" is caught.
- **Five-second rule** — when the opening moment ends, is the phone number / booking / price on screen?

---

## Notes

- Every rule here is a *default* to break deliberately, not a law. Breaking one on purpose, with a reason you can state, is design. Breaking one by reflex is slop.
- The order section is the part people skip. It is also the part that decides whether the rest can work.
