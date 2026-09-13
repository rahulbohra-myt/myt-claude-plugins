# MyYogaTeacher Claude Plugins

Internal Claude plugin marketplace for MyYogaTeacher (MYT). Main plugin:
`plugins/myt-lp-product-copy` — generates on-brand copy for landing pages and website pages,
used by the content & SEO team and any MYT teammate.

This file guides *building* the plugin. Installed plugins don't read it — anything team members
need at runtime must live in the plugin's skills and references.

## What the plugin does

MYT serves two audiences: **students** (live online yoga — ~90% of pages) and **teachers**
(hired onto the platform to teach).

| Category | Side | Typical CTA destination |
|---|---|---|
| Paid ad LP (Meta / Google) | Student | Combined Funnel Onboarding — name + WhatsApp form in the hero (required) |
| Free event LP — weekly sessions, quarterly main events (most-used event category) | Student | Registration form, usually in the hero; other CTAs scroll to it |
| Workshop LP, free or paid (e.g. nutrition) — less common | Student | Registration / payment |
| TTC workshop LP | Teacher | Registration |
| Teacher hiring LP (Meta ads) | Teacher | Typeform |
| Website page (home, services, product, about, contact) | Mostly student | Varies; homepage uses Combined Funnel Onboarding |

Every generation follows this workflow (implemented in `skills/myt-page-copy`):
1. **Intake** — side, category, goal, traffic source, CTA + destination, tone, available assets.
   Ask until the important items are clear; never re-ask what's answered.
2. **Outline** — sections and order from the category playbook, built from the section library,
   with heading hierarchy and word targets. Confirm with the user.
3. **Generate** — copy every section to its template and Brand Core rules.
4. **Feedback** — ask for feedback, revise, repeat until the user is satisfied.

Popups, banners, product cards and similar one-off assets go to `skills/myt-product-feature-copy`.

## Sources of truth — never duplicate

All paths below are under `plugins/myt-lp-product-copy/`.

- `references/MYT_Brand_Core.md` — terminology, tone, CTA microcopy, platform figures, disclaimers,
  conversion heuristics (Track A SEO-blended vs Track B pure conversion).
- `references/LP_Section_Library.md` — every section/component: elements, hierarchy, word counts.
- `references/playbooks/` — per-category section recipe + category-specific intake.
- `references/Teacher_Hiring_Context.md` — eligibility, onboarding, earnings facts.
- `references/examples/<category>/` — real shipped copy for calibration.

Skills point to these files. Never copy rules, figures, or section templates into a skill.

## Rules for changing the library and playbooks

- Components are category-neutral. Playbooks *pick and order* components; they don't own them.
- Before adding a component, check whether it's genuinely new or an existing one with different
  copy — ask if unsure. (Easy to Get Started ≠ How It Works: onboarding steps vs ongoing experience.)
- Every template cites its source (Figma node or live URL). Word counts come from shipped pages.
- Figma (`Branding-page-updates`, file key `Gd0skTKGGWundB5QBRqj65`) lags production — the paid-LP
  hero's name + WhatsApp form was missing there. Confirm against a live page or screenshot.
- If a category has no or thin examples, ask for real shipped copy before inventing recipes or word
  counts; mark anything built without examples as provisional.
- Brand Core banned terms apply everywhere, including examples in templates ("coach", "coaching").
- Out of scope: nav bar, footer, dynamic widgets (e.g. live "recent bookings" strip).

## Repo mechanics

- Marketplace manifest: `.claude-plugin/marketplace.json`; each plugin has
  `.claude-plugin/plugin.json`. Register new plugins in the marketplace manifest.
- The repo is GitHub-synced to the org marketplace — pushing to `main` releases to the whole team.
  Confirm before pushing; bump `version` in both manifests when skills or references change.
- Owner: Rahul Bohra.
