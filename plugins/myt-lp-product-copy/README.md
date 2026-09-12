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
- `LP_Section_Library.md` — the single source of truth for landing page **section structure**:
  a numbered standard sequence (Hero Section, Logo Mark, Benefits Grid, Benefit Section, How It
  Works, Text Testimonials, Expert Teachers, Comparison Table, Video Testimonials, Eligibility
  Checklist, Easy to Get Started, FAQ Section, Landing CTA) plus optional/supplementary
  components (Use Cases, Testimonials Alternate, For Your Unique Needs). See the file itself
  for the current, authoritative list and per-section templates — don't duplicate the list
  here, it will drift. Each template is category-neutral — not owned by paid LPs, events,
  teacher recruitment, or any other page type — so every LP-generating skill sequences and
  adapts from it rather than holding its own copy of the same section. Excludes the nav bar,
  footer, and any dynamic/data-driven widgets (e.g. a live "recent bookings" strip) since those
  aren't generated copy.
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

Two files are the sources of truth every skill defers to, instead of holding its own copy:

- `MYT_Brand_Core.md` — brand language, tone, and standing figures.
- `LP_Section_Library.md` — landing page section structure and word/character targets.

Update these when brand rules or section templates change; this is the drift this plugin was
built to fix in the first place.
