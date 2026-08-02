# MyYogaTeacher — Landing Page & Product/Feature Copy

Generates on-brand first-draft copy for MyYogaTeacher landing pages and product/feature assets.
Built for teams outside SEO (paid ads, growth, recruitment, product) who need on-brand copy
without needing MYT's full company context loaded first — everything this plugin needs is
bundled inside it.

## What's inside

**`references/`**
- `MYT_Brand_Core.md` — the single source of truth every skill below reads before drafting:
  approved/prohibited terminology, tone by content type, standard CTA/microcopy, standing
  platform figures, medical disclaimer copy, and conversion-copywriting heuristics.
- `examples/paid-lps/` — real paid-campaign LP copy for calibration *(add files here)*
- `examples/teacher-hiring-lps/` — real teacher-recruitment LP copy for calibration *(add files here)*

**`skills/`**

| Skill | Use for |
|---|---|
| `about-myyogateacher` | Company/audience context |
| `myt-lp-generator` | Paid ad landing pages (condition-led, audience, lifestyle, style) — already ships with 2 reference examples (`flexibility-lp-copy.md`, `prenatal-lp-copy.md`) |
| `myt-lp-event-generator` | Event/workshop landing pages |
| `myt-teacher-hiring-context` | Teacher recruitment landing page context |
| `myt-product-feature-copy` | Popups, in-app banners, product cards, brochures, communication docs — runs a short intake Q&A first since there's no fixed template for this category |

## Out of scope, by design

- **Articles/taxonomy content** — separate plugin, not yet built
- **LP → shippable Astro code** (`lp-astro-generator`) — separate plugin, planned for later
- **Google Ads campaign audits** (`google-ads-audit`) — a diagnostic tool, different job from copy generation, kept separate

## How to use

Just describe what you need — e.g. *"write a landing page for a sciatica-relief ad campaign"* or
*"I need popup copy for our new referral feature."* The relevant skill asks a few clarifying
questions before drafting (audience, word count, must-include elements) and always checks
terminology and tone against `MYT_Brand_Core.md` first.

## Maintenance

`MYT_Brand_Core.md` is the one file to update when brand language, tone, or standing figures
change — skills should reference it rather than hold their own copy of any rule, to avoid the
kind of drift this plugin was built to fix in the first place.
