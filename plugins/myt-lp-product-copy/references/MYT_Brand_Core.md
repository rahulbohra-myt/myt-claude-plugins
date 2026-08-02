# MyYogaTeacher — Canonical Brand Core
**Version:** 1.0 (locked)
**Owner:** Rahul Bohra
**Last updated:** August 2026 (v1.3)
**Purpose:** Single source of truth for brand voice, terminology, audience, and compliance rules. Every content-generation skill in the MYT plugin(s) should reference this file rather than embedding its own copy of brand rules — that's what keeps future updates from drifting out of sync across skills.

---

## 1. Company Snapshot

MyYogaTeacher is an online yoga platform connecting students with expert Indian yoga teachers for live, interactive sessions delivered via Zoom — both 1-on-1 and small group classes. Available via web (myyogateacher.com) and mobile app.

**Differentiator:** Authentic traditional Indian yoga, not westernized fitness yoga — live, personal, and culturally rooted.

**Business model:** 3-day free trial → subscription (1-on-1 + group class options).

**Positioning line:** First global platform connecting Indian yoga teachers with students worldwide for live 1-on-1 sessions.
**Brand line:** *"Rooted in tradition. Powered by technology. Driven by community."*

---

## 2. Audience Segments

### 2.1 Students (primary content audience)
- **Core:** Indian diaspora abroad — proud of cultural roots, values authentic teaching
- **Age:** 35–65 (some 65+) · **Gender split:** ~70% women, ~30% men
- Married with children; many in the "sandwich generation" (caring for kids + elderly parents)
- Busy professionals, time-constrained, predominantly sedentary
- Self-conscious in gyms/studios; past failed attempts (YouTube, gym memberships) created hesitation
- **What they want:** personalized guidance for their specific body, judgment-free accountability, cultural trust, schedule flexibility, a gentle re-entry into movement

**Key messages to echo:**
- "Someone who understands my body and my challenges"
- "Authentic yoga, not just fitness"
- "Guidance I can trust — from teachers who really know yoga"
- "Something that fits my schedule, not the other way around"

### 2.2 Prospective Teachers (recruitment content audience)
- Value pillars: earnings (marketplace-based, not guaranteed), flexibility, marketing/tech handled by MYT, community, global reach, purpose
- Closing line: *"Your passion. Your expertise. Your schedule. Your global classroom."*
- Tone runs more aspirational/mission-driven than student-facing copy, but stays warm — never salesy or corporate
- Full eligibility, earnings, onboarding data lives in the `myt-teacher-hiring-context` skill — this doc doesn't repeat it

### 2.3 Markets
| Market | Priority |
|---|---|
| United States | Primary |
| Canada, UK, Australia | Secondary — active content focus |
| UAE, Saudi Arabia | Secondary — lower content priority |

---

## 3. Terminology — ✅ Confirmed

**Approved:** "expert," "certified," "1-on-1," "personalized"
**Prohibited (customer-facing copy):** "coach," "coaching," "real," "private," "personal"

"Certified" is approved and should be used where it strengthens the differentiator — e.g. "certified Indian yoga teachers." It also applies internally as-is (teacher eligibility criteria in `myt-teacher-hiring-context` — 300+ hours TTC, etc.) with no distinction needed between internal and customer-facing use.

**"Coach"/"coaching" — no exceptions.** Confirmed: this ban applies to all customer-facing copy with zero carve-outs, including individual teacher specialization titles (e.g. do not write "Fitness Coach," "Wellness Coach," "Therapeutic Yoga Coach" — use "teacher" or a specialization phrase built around "teacher"/"expert" instead).

| ❌ Never use | ✅ Use instead |
|---|---|
| coach / coaching | teacher |
| real | expert / certified |
| private | 1-on-1 |
| personal | personalized |

### 3.1 Standard CTA & Microcopy (confirmed from live homepage)

The homepage uses one consistent CTA pattern at every conversion point — primary button + a fixed reassurance line directly beneath it, repeated identically rather than varied:
- **Button text:** "Book a free session"
- **Paired microcopy:** "No Credit Card Required"

For longer-form CTA copy (meta descriptions, ad headlines, LP hero subtext) where more context fits: "Book a free 1-on-1 session with a certified, expert Indian yoga teacher."

### 3.2 Live-Site Violations Found (reference only — not an active workstream)

A live-page audit (Aug 2026) found the terminology rules above weren't yet reflected on the current site: About Us meta title/description used "coaching" and "Real yoga"; several homepage teacher bios used "Coach" as a job title; the homepage comparison table had a row labeled "1-on-1 Coaching." **Deprioritized as of Aug 2026 — old content, not an active cleanup task.** Kept here only so it doesn't get mistaken for approved precedent if anyone references the live site while drafting new copy.

---

## 4. Tone & Voice by Content Type

| Content type | Tone | Notes |
|---|---|---|
| General / student-facing (articles, taxonomy pages) | Warm, encouraging, culturally resonant, judgment-free | Never aggressive-fitness or westernized-wellness-buzzword |
| Condition-led / YMYL-adjacent | Same warmth, plus medically careful — no overclaiming, no diagnostic language | Disclaimer mandatory (see §6) |
| Teacher recruitment | Aspirational, mission-driven, still warm — never corporate/salesy | Pair any earnings figure with the marketplace framing rule in `myt-teacher-hiring-context` |
| Events / workshops | Warm + a genuine urgency/community layer (time-bound, cohort framing) | Confirm: I haven't seen a dedicated tone note for events beyond what's embedded in `myt-lp-event-generator` — worth double-checking that skill's assumptions still match this table |
| Philosophy / spiritual | Warm, respectful of tradition, avoids appropriation-flavored language | Lean on "Authentic Indian Yoga Teaching" framing from the content mind map |

**Framing rule that applies everywhere:** "Yoga for [condition]" outperforms "Yoga poses for [condition]" for conversion — default to the condition-first framing unless the content is explicitly a poses roundup.

---

## 5. Content Pillars

1. Condition-Led / Pain & Health
2. Chakras & Energy Centers
3. Yoga Styles & Comparisons
4. Poses & Stretches
5. Pranayama & Breathwork
6. Weight Loss & Fitness
7. Mental Health & Stress
8. Life Stage
9. General Wellness & Lifestyle
10. Philosophy & Spiritual

The full topic-level mind map (hundreds of specific angles under each pillar) lives in `MYT_Content_Pillars_Mind_Map` in project knowledge — treat the 10 pillars above as the organizing structure any new topic gets sorted into.

---

## 6. Medical / YMYL Disclaimer Rules

- **Mandatory** on all condition-led / pain & health content — articles, taxonomy sections, and any LP/product copy that references a specific health condition.

**Drafted standard disclaimer (recommend a legal review pass before treating as final — I'm not a lawyer and this is copywriting judgment, not legal sign-off):**

**Short form** (inline, directly below H1/hero on condition-led pages):
> Yoga can support your wellbeing, but it isn't a substitute for medical care. Check with your doctor before starting a new practice — especially if you're managing an existing health condition.

**Full form** (dedicated callout box, e.g. before the FAQ or at the top of a condition-led article):
> **A note before you begin:** The information here is for general educational purposes and isn't intended as medical advice, diagnosis, or treatment. Yoga can be a valuable complement to your health routine, but it doesn't replace care from a qualified healthcare provider. If you have an existing condition, are pregnant, or are recovering from an injury, please check with your doctor before starting a new practice.

Use the short form on LP/product pages where space is tight; use the full form on long-form condition-led articles. Both avoid clinical/alarming language to stay consistent with the warm brand voice, while still being direct about the "not medical advice" point.

---

## 7. Authorship / E-E-A-T Rules

- Named, credentialed reviewer paired with the "MyYogaTeacher" org byline is the recommended approach — stronger for E-E-A-T than org byline alone.
- Author byline changed from named authors → org byline at end of March 2026; flagged as a possible factor in impression drops. Any new author-strategy content should account for this rather than assume the pure org-byline approach is settled policy.

---

## 8. Standing Approved Platform Figures

**Confirmed current (Aug 2026):**
- 240,000+ students · 372,000+ sessions · 450+ teachers · 100+ GC Classes Daily · 4.9★ rating

**Freshness rule:** these numbers grow over time — treat them as a floor, not a fixed fact. Before inserting any of these figures into new LP or product copy, confirm the current number rather than assuming this doc is still accurate at the time of use. This is what caused the 200+/360+ teacher-count and 300,000/372,000-session discrepancies found in the last audit — don't let it happen again with stale hardcoded figures downstream.

**Also observed on the live homepage (not standing figures, situational/descriptive use only):**
- Press-mention trust bar: Woman's World, Well+Good, Women's Health, LA Yoga, Yahoo Life, Men's Health magazines

⚠️ **Note:** `myt-teacher-hiring-context` skill still lists its own standing figure as "360+ teachers" — that's now stale against the confirmed 450+ above. Worth updating that skill file to match, or better, having it reference this doc instead of holding its own copy of the number.

---

## 9. Conversion-Copywriting Heuristics

This section is separate from SEO rules on purpose — it's a different discipline, applied differently depending on what kind of page you're writing.

### 9.1 Two Tracks — Not One Ruleset

| | **Track A — SEO-Blended** | **Track B — Pure Conversion** |
|---|---|---|
| **Applies to** | Homepage, commercial/service pages (group classes, teacher directory, pricing if it's meant to rank) | Paid LPs, event/workshop LPs, teacher-recruitment LPs, in-app product/feature pages |
| **Primary job** | Rank organically *and* convert once someone lands | Convert a visitor who already clicked an ad or link — nothing to rank |
| **Keyword handling** | Primary keyword still required in H1/title/meta; header hierarchy still matters | No keyword-density constraint — write for the one reader in front of you, not a query |
| **Success test** | Does it satisfy both a search engine and a human? | Does it satisfy the promise that got them here, as fast as possible? |
| **Governing discipline** | SEO Expert Prompt rules (existing) + conversion layer on top | Conversion-copywriting heuristics below, close to fully |

The homepage is Track A in practice — it has a keyworded H1 ("Online Yoga Classes with Expert Indian Teachers - Live!") *and* the full conversion toolkit (comparison table, objection FAQ, trust stack). That's the model for other Track A pages. Track B pages should feel lighter and more single-minded — one promise, one CTA, nothing competing for attention.

### 9.2 Core Heuristics

| Heuristic | What it means in practice | Where it comes from |
|---|---|---|
| **Message match** | LP copy must mirror the exact promise/headline in the ad or link that drove the click — any gap between ad and page kills conversion and hurts Quality Score | Oli Gardner (Unbounce) — directly relevant given `google-ads-audit` already tracks ad→LP→offer alignment |
| **Above-the-fold value proposition** | Who it's for + what they get + proof + one action, visible without scrolling | Donald Miller (*StoryBrand*), April Dunford (*Obviously Awesome*) |
| **Benefit over feature ("so what?" test)** | Keep translating a feature until you hit a felt outcome — "200+ teachers" → "never stuck waiting for one person's schedule" | David Ogilvy; Eugene Schwartz, *Breakthrough Advertising* |
| **Classic structural formulas** | AIDA (Attention–Interest–Desire–Action) for full pages; PAS (Problem–Agitate–Solve) for shorter/ad copy | AIDA traced to E. St. Elmo Lewis (1898); PAS is direct-response staple |
| **Clarity over cleverness** | Plain words, short sentences, no jargon — never make the reader re-read a line | Steve Krug, *Don't Make Me Think*; Ann Handley, *Everybody Writes* |
| **Contrast/reframe device** | "It's not about X — it's about Y" defuses an objection before it's raised (MYT already does this: "isn't about judgment, it's about support") | Direct-response tradition (Schwartz, Halbert) |
| **Objection-handling FAQ + risk reversal** | Answer skepticism directly ("how are you this affordable?"), pair any ask with a risk-reducer ("no credit card required") | Gary Halbert; Claude Hopkins, *Scientific Advertising* |
| **Social proof & the 6 principles of persuasion** | Testimonials, numbers, ratings, press logos — stacked, not one-and-done | Robert Cialdini, *Influence* |
| **Scannability / reading pattern** | Bullets, subheads, bold labels, short paragraphs — people scan in an F-pattern, they don't read top to bottom | Jakob Nielsen (Nielsen Norman Group) |
| **Single clear CTA** | One primary action per page/section; every extra choice is friction | Hick's Law; Oli Gardner's "Attention Ratio" concept |
| **Ultra-specific numbers beat vague claims** | "240,000+ students" beats "thousands of happy students" | Michael Masterson's "4 U's" headline formula (Urgent, Unique, Ultra-specific, Useful) |
| **Concrete + emotional > abstract** | "Ease back pain, neck tension, and joint stiffness" beats "improve your wellbeing" | Chip & Dan Heath, *Made to Stick* (SUCCESS framework) |
| **Positioning via direct comparison** | Argue differentiation visually (a table), not in paragraphs | April Dunford, *Obviously Awesome* |
| **Conversion copywriting as its own tested discipline** | Treat copy as a hypothesis to test, not a one-shot draft | Joanna Wiebe (Copyhackers — coined "conversion copywriting"); Peep Laja (CXL) |
| **Microcopy consistency** | Same CTA button text + reassurance line everywhere, not reworded per page | Kinneret Yifrah, *Microcopy: The Complete Guide*; Torrey Podmajersky, *Strategic Writing for UX* |

### 9.3 Practical Checklist by Track

**Track A (Homepage/commercial pages):** keyword in H1 → value prop above the fold → benefit-led section headers → comparison table if a direct competitor framing exists → objection-handling FAQ → trust stack (numbers + press + rating) → schema markup per SEO rules.

**Track B (LP/Product-Feature pages):** confirm message match with the source ad/link first → one value prop, one CTA repeated → benefit-led, not feature-led → risk reversal near every ask → skip keyword optimization entirely — optimize for the one promise that got them here.

---

## 10. Governance

- **Owner:** Rahul Bohra — single point of update for this file.
- **Update rule:** Any brand-language, tone, or compliance change gets made here first, then propagates to skills — never patched directly in an individual skill file. That's the mechanism that prevents the drift we found in Section 3 from happening again.
- **Version history:**
  - v0.9 (Aug 2026) — initial consolidation draft; Section 3 pending sign-off
  - v1.0 (Aug 2026) — locked; Section 3 terminology confirmed ("certified" restored as approved, applies internally and customer-facing)
  - v1.1 (Aug 2026) — confirmed "coach"/"coaching" has zero exceptions (incl. teacher bio titles); added standard CTA/microcopy pattern (§3.1); flagged live-site terminology violations (§3.2); added homepage-confirmed platform figures and a teacher-count/session-count discrepancy vs. the teacher-hiring standing figures (§8)
  - v1.2 (Aug 2026) — updated standing figures to confirmed current numbers (450+ teachers, 100+ GC classes daily); added freshness rule requiring confirmation before reuse; drafted standard medical disclaimer copy (§6, short + full form); live-site cleanup marked deprioritized per Rahul, not an active workstream
  - v1.3 (Aug 2026) — added Conversion-Copywriting Heuristics (§9): two-track model (SEO-blended vs. pure-conversion pages), core heuristics with named frameworks, practical checklist per track

