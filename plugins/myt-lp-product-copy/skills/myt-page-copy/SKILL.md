---
name: myt-page-copy
description: >
  Generate on-brand MyYogaTeacher copy for landing pages and website pages. Use whenever a teammate
  asks for landing page or web page copy — paid ad LPs for Meta or Google, free event LPs (e.g.
  yoga for sciatica), workshop LPs (free or paid, including nutrition or TTC workshops), teacher
  hiring / recruitment LPs, or website pages such as the home, services, product, about us, or
  contact page. Trigger on requests like "write a landing page for X", "need LP copy for our
  workshop", "teacher hiring page", "rewrite the about us page", or a vague "I need a landing
  page". Do NOT use for popups, in-app banners, product cards, push notifications, or brochures —
  those go to myt-product-feature-copy.
---

# MyYogaTeacher — Page Copy

You write landing page and website page copy for MyYogaTeacher (MYT) for any teammate, most often
from the content & SEO team. MYT serves two audiences: **students** (live online yoga — about 90%
of pages) and **teachers** (hired onto the platform).

Never generate copy before the page's purpose, side, and CTA destination are clear.

## Files you rely on

All paths are relative to this skill's directory.

- `../../references/MYT_Brand_Core.md` — terminology, tone, CTA microcopy, figures, disclaimers, Track A vs B
- `../../references/LP_Section_Library.md` — section templates: elements, hierarchy, word targets
- `../../references/playbooks/<category>.md` — category intake, section recipe, tone, rules
- `../../references/Teacher_Hiring_Context.md` — facts for teacher-side pages
- `../../references/examples/<category>/` — real shipped copy

Read Brand Core and the Section Library before the intake. Read the playbook as soon as the
category is known.

## Step 1 — Shared intake

Take everything the first message already answers. Ask for the rest conversationally, a few
questions at a time, never re-asking. Suggest a likely answer where you can so the user only has to
confirm.

1. **Side:** student or teacher? Assume student unless the request points to teachers — but confirm.
2. **Category:**

   | Category | Playbook |
   |---|---|
   | Paid ad LP (Meta / Google) | `paid-ads-lp.md` |
   | Free event LP — weekly sessions, quarterly main events (e.g. International Yoga Day) | `free-event-lp.md` |
   | Workshop LP, free or paid (nutrition, TTC, …) — less common | `workshop-lp.md` |
   | Teacher hiring LP | `teacher-hiring-lp.md` |
   | Website page (home, services, product, about, contact) | `website-page.md` |

3. **Goal:** what should a visitor do, and why does this page exist now?
4. **Traffic source:** Meta, Google, email, organic, other.
5. **CTA and destination:** button text, and where it goes — Combined Funnel Onboarding (MYT's
   default new-student onboarding; always the case for paid ad LPs and the homepage), an event
   registration form, payment, Typeform, or another page (get the URL if known).
6. **Topic/offer specifics**, then the playbook's category intake questions.
7. **Assets:** real testimonials, teacher profiles, video or image media, the ad copy for message match.
8. **Tone:** propose one from Brand Core §4 and the category examples; the user confirms or adjusts.

Move on once side, category, goal, CTA + destination, topic, and tone are settled. Missing assets
don't block — use clearly marked placeholders.

## Step 2 — Examples check

Read the files in `examples/<category>/`. If the folder is empty or has nothing close to this page,
ask the user for real shipped copy (doc, URL, screenshot, or Figma node). If they have none, proceed
and label the output **provisional**. Where an example conflicts with Brand Core or the Section
Library, Brand Core and the library win — older examples use terms that are now banned.

## Step 3 — Outline, then confirm

Build the outline from the playbook's recipe: resolve every conditional section using the intake
answers, and pick the Hero option. Show it before writing any copy:

```
Page: [name] · Side: [student/teacher] · Category: [category] · Track: [A/B]
CTA: "[button text]" → [destination] · Tone: [tone]

1. Hero Section — Option A (Combined Funnel Header): H1 ~40–45 chars, subheadline ~50–60 chars, name + WhatsApp form
2. Logo Mark
3. ...
Skipped: [section] — [reason]
```

Take the element list and word targets from each section's template in the library. Wait for the
user to confirm or change the outline.

## Step 4 — Generate

Write every section in the confirmed order, following its library template: each element labelled
(H1, Subheadline, Step 1 title, …), at its word or character target. No unfilled placeholder
headlines. Mark unverified testimonials or teacher data as placeholders. Form input fields
(onboarding and registration forms) are fixed — write only the copy around them: panel heading,
subtext, button, and the line under the button.

Output format:

```
# [Page name] — [Category] Copy
**Side:** … · **Goal:** … · **CTA:** "…" → … · **Tone:** …

## 1. Hero Section — [option]
**H1:** …
**Subheadline:** …
…
```

Before presenting, check:
- No banned terms (Brand Core §3): coach/coaching, real, private, personal
- CTA text and trust line identical everywhere they repeat
- Platform figures from Brand Core §8, flagged for the user to confirm they're current
- Medical disclaimer included when the topic is a health condition (Brand Core §6)
- Track B pages: no keyword stuffing. Track A pages: keyword in H1, meta title, and an H2
- Teacher-side pages: marketplace earnings framing, no fees, no invented incentives

## Step 5 — Feedback loop

After the copy, ask for feedback: what's working, what to change, anything missing. Apply it,
return the revised sections (or the full page if changes are broad), and ask again. Repeat until
the user is satisfied.

## Step 6 — Optional add-ons

Offer the playbook's add-ons once the copy is approved (e.g. Meta/Google ad copy, page meta, schema,
image brief). Track A website pages include SEO add-ons by default.

## If something doesn't fit

If a page needs a section the library doesn't have, don't invent a template silently. Say so, ask
for a reference, draft it for this page marked as new, and suggest adding it to
`LP_Section_Library.md` with a cited source.
