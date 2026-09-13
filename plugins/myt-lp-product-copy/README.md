# MyYogaTeacher — Page Copy & Product/Feature Copy

Generates on-brand first-draft copy for MyYogaTeacher landing pages, website pages, and
product/feature assets. Built for the content & SEO team and any MYT teammate — everything the
plugin needs is bundled inside it.

## Skills

| Skill | Use for |
|---|---|
| `myt-page-copy` | Landing pages and website pages — paid ad LPs (Meta/Google), free event LPs, workshop LPs (free/paid, incl. TTC), teacher hiring LPs, home/services/product/about/contact pages |
| `myt-product-feature-copy` | Popups, in-app banners, product cards, push notifications, brochures, communication docs |

## How `myt-page-copy` works

1. **Intake** — student or teacher side, category, goal, traffic source, CTA and where it goes,
   topic, assets, tone. It asks only what your first message didn't cover.
2. **Examples check** — reads real shipped copy for the category; asks you for some if there's none.
3. **Outline** — proposes the sections, their order, and word targets. You confirm.
4. **Copy** — writes every section to the template and brand rules.
5. **Feedback** — revises until you're happy, then offers add-ons (ad copy, page meta, schema).

Try: *"Write a Meta ad landing page for yoga for sciatica"*, *"We need a teacher hiring page for
yoga therapy teachers"*, or just *"I need a landing page"*.

## References

```
references/
  MYT_Brand_Core.md          brand voice, terminology, CTA microcopy, figures, disclaimers
  LP_Section_Library.md      every section template: elements, hierarchy, word targets
  Teacher_Hiring_Context.md  eligibility, onboarding, earnings facts for teacher-side pages
  playbooks/                 per-category intake + section recipe
    paid-ads-lp.md  free-event-lp.md  workshop-lp.md  teacher-hiring-lp.md  website-page.md
  examples/                  real shipped copy per category (see examples/README.md)
```

**Calibration status:** paid ad LPs and teacher hiring LPs are calibrated against shipped pages.
Free event, workshop, and website page playbooks are provisional until real examples are added to
`references/examples/`.

## Out of scope, by design

- Articles/taxonomy content — separate plugin, not yet built
- LP → shippable Astro code — separate plugin, planned
- Google Ads campaign audits — separate diagnostic tool

## Maintenance

See `CLAUDE.md` at the repo root for how to change the library, playbooks, and examples.
