---
name: myt-product-feature-copy
description: >
  Generate first-draft copy for MyYogaTeacher product/feature assets that aren't landing pages
  or articles — popups, in-app banners, product cards, push notifications, feature announcements,
  communication documents (emails, memos), brochures, and similar one-off assets. There's no fixed
  template for this category (unlike LP or taxonomy pages), so this skill runs a short intake
  before drafting rather than assuming a brief already exists. Trigger whenever a teammate asks
  for copy for an app popup, in-app message, product card, push notification, feature announcement,
  brochure, or similar — including vague or informal requests like "need copy for our new referral
  feature" where the format isn't yet specified. Always reference MYT_Brand_Core.md for
  terminology, tone, and CTA rules before drafting.
---

# MyYogaTeacher — Product/Feature Copy Generator

For one-off product/feature copy that doesn't fit the landing-page or article pipelines: popups,
in-app banners, product cards, push notifications, brochures, feature announcements,
communication docs. There's no existing template for this category — the skill's job is to run a
short, friendly intake before drafting, since teammates requesting this today do so informally
(ad hoc Slack/email asks, no brief format).

## Step 0 — Always Load Brand Core First

Before anything else, reference `MYT_Brand_Core.md`:
- **Terminology (§3)** — "coach"/"coaching" banned with zero exceptions; "certified" approved
- **Standard CTA/microcopy (§3.1)** — "Book a free session" / "No Credit Card Required" as defaults, unless the format calls for something else
- **Tone by content type (§4)**
- **Standing platform figures (§8)** — confirm the current number before using any stat; don't reuse a hardcoded figure from memory
- **Conversion-copywriting heuristics (§9)** — this content is almost always **Track B** (pure conversion / UX-first): no keyword constraint, optimize purely for the reader encountering this one asset

## Step 1 — Intake (ask only what's still missing)

Most requests arrive as an informal one-liner (e.g. "need copy for a popup about our new referral
feature") — there's no brief format teammates are used to filling out, so don't wait for one. Take
whatever's given, then ask conversationally for whatever's still missing from:

1. **What are you creating?** (popup / in-app banner / product card / push notification / brochure / communication doc / other — ask them to describe if "other")
2. **What's it for** — one sentence on the goal
3. **Where will the reader encounter it?** (in-app, email, PDF handout, website widget) — this drives tone/format more than the asset type alone
4. **Word/character constraint** — an exact number if they have one; if not, propose a default from Step 2 and confirm
5. **Audience** — new students, existing students, prospective teachers, other
6. **Any must-include elements** — a specific stat, CTA, feature name, policy detail
7. **An existing example to match**, if one exists

Skip anything already answered in the initial request — don't re-ask.

## Step 2 — Format Defaults (starting points, always confirm rather than assume)

| Format | Typical length | Notes |
|---|---|---|
| Push notification | ~40–90 characters | Front-load the benefit; platform truncates aggressively |
| Popup / in-app banner | 1 headline + 1–2 sentence body | One CTA only |
| Product card | Title + 1–2 line description | No room for a full value-prop paragraph |
| Feature announcement (in-app or email) | 100–250 words | Benefit-led, one primary CTA |
| Brochure / PDF handout | Varies widely | Ask for page count or word target explicitly — don't assume |
| Communication doc (internal memo, teacher-facing update) | Varies | If teacher-facing, match tone guidance in `myt-teacher-hiring-context` |

These are proposed starting points for the intake conversation, not hard rules — always confirm
against what the requester actually needs rather than locking to the table.

## Step 3 — Draft

Produce **one draft**, not multiple strategic variants (confirmed preference — this differs from
`myt-lp-generator`, which produces variants; this skill doesn't). Apply brand core terminology and
tone rules throughout.

If the copy touches pricing, cancellation, free-trial terms, or other policy specifics: don't
invent exact figures or policy language from memory — flag anything uncertain for the requester to
confirm. This category isn't YMYL-level (no medical disclaimer required), but a wrong stated policy
detail is still a real problem, just a lower-stakes one to catch.

## Step 4 — Feedback Pass

Present the draft with a short prompt for feedback (what's working, what to change, anything
missing) before calling it final. One revision round is the expected norm — surface the revised
draft back to the requester rather than iterating silently.
