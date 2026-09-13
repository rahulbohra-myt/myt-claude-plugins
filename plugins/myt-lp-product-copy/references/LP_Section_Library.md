# MYT Page Copy — Section Library

Shared, reusable templates for every section/component used on MyYogaTeacher landing pages and
website pages. Components are **not** owned by any page category — category playbooks in
`playbooks/` pick and order them. Never copy a template into a skill or playbook; point to it.

**Out of scope:** the site navigation bar, the footer, and dynamic widgets (e.g. a live "recent
bookings" strip) — fixed or data-driven, never generated as copy.

**Calibration sources** — word/character counts are realistic targets from shipped pages, not hard caps:
- Figma `Branding-page-updates` (file key `Gd0skTKGGWundB5QBRqj65`): Prenatal page (node 7635-5187),
  Hormonal Balance & Women's Health (10352-78), Back Pain V1 (5006-944), Prenatal teacher
  recruitment (10062-5814)
- Live production paid-LP hero screenshot (Flexibility, Sep 2026)
- Free event: live page `myyogateacher.com/events/yoga-for-sciatica` + Figma `Event-Page` (file key
  `v2qJ9xybT22QBDwbMbr4ou`, node 2-2202 — dummy copy, structure only)
- Shipped copy docs in `examples/`

Figma lags production — confirm against a live page before recalibrating from Figma alone.
Components marked **⚠️ Provisional** have no shipped source yet; recalibrate them when examples arrive.

---

## Component Index

| # | Component | Typical use |
|---|---|---|
| 1 | Hero Section (Option A Combined Funnel Header / Option B Media Hero) | Student pages — Option A required on paid ad LPs and the homepage |
| 2 | Logo Mark | Every page |
| 3 | Benefits Grid Section | Broad topics with sub-needs; teacher hiring "why teach" |
| 4 | Benefit Section | Most pages |
| 5 | How It Works | Ongoing service experience |
| 6 | Text Testimonials | Most pages |
| 7 | Expert Teachers | Most pages |
| 8 | Comparison Table | Paid LPs, service pages |
| 9 | Video Testimonials | Most pages |
| 10 | Eligibility Checklist | Recruitment / application / prerequisite pages |
| 11 | Easy to Get Started | Onboarding / application steps |
| 12 | FAQ Section | Every page |
| 13 | Landing CTA | Every page |
| 14 | What's Included ⚠️ | Events, workshops |
| 15 | Event Details Card ⚠️ | Events, workshops |
| 16 | Pricing Block ⚠️ | Paid workshops |
| 17 | Event Registration Hero | Event pages |
| 18 | Meet {Teacher} | Pages led by one teacher (events) |
| — | Optional: Use Cases, Testimonials — Alternate Format, For Your Unique Needs | Any page |

Order on a page comes from the category playbook, not from these numbers.

---

## 1. HERO SECTION

Two coequal options for the same slot — pick one per page. Which one depends on whether the page's
strongest asset is aggregate social proof or a compelling piece of media.

### Option A — Combined Funnel Header

The hero for **Combined Funnel Onboarding** — MYT's default new-student onboarding flow. Stat-based
trust signals plus an inline name + WhatsApp form that starts onboarding. **Required on every paid
ad LP**, and used on the homepage. (Confirmed from a production screenshot; the Figma frames lagged
and lacked the form.)

```
### H1 (Main Headline):
**[Keyword/benefit-led. ~40–45 chars. Names the topic/program and the core promise. e.g.
  "1-on-1 Online Yoga Classes for Flexibility"]**

### H1 (Alternative for A/B Testing):
**[Word-order variant or identity/outcome reframe. Different structure from primary H1.]**

### Subheadline:
[Benefit-led expansion, ~50–60 chars. e.g. "Build Flexibility and Strength with Personalized Yoga"]

### Lead Capture Form (inline — the CTA lives here, not as a standalone button):
- Name field — placeholder text: "Your name"
- Phone field — country-code selector (flag + dial code dropdown) + placeholder text:
  "Your WhatsApp number"
- Submit button (this IS the primary CTA): **[Verb set by the playbook — e.g. "Book a free session"]**

### Trust Line:
[Directly beneath the form — e.g. "No Credit Card Required".]

### Trust Bar (2–3 stat items, laurel/badge style):
- [N]K+ 5 star ratings
- 4.9 App Store
- [optional third — e.g. press mention]

### Hero Visual:
[Full-bleed lifestyle/mood photo background — person, setting, expression, pose. No text baked
 into the image; H1/subheadline/form render on top of it.]
```

**Form field copy stays fixed** ("Your name" / "Your WhatsApp number") — only the submit button's
verb changes per page goal.

**Button-only layout (teacher hiring):** the shipped prenatal teacher recruitment page uses this
layout with a single "Apply Now" button → Typeform in place of the form. That page isn't Combined
Funnel Onboarding — it only borrows the layout.

### Option B — Media Hero Section

_Source: Figma node 5006-944 — "Back Pain - V1 - No video"._

The media is the section's main trust-building device, so it's the first field.

```
### Hero Visual — Video or Image (required, defines this option):
[A live-session preview, not a generic lifestyle photo: framed like an in-progress Zoom call.
 Include a "LIVE" badge, an in-call control bar (mute/camera-style icons), and a name tag
 identifying the teacher (label it "Teacher"). Works as a static image or a video loop —
 the surrounding copy is identical either way.]

### H1 (Main Headline):
**[Keyword/benefit-led. ~30–40 chars — shorter than Option A, no A/B alt. e.g.
  "1-on-1 Yoga At Home for Back Pain"]**

### Subtext:
[One short line, ~5–7 words / ~30–40 chars, naming the format — e.g. "With an Expert Teacher,
 Live via Zoom".]

### Primary CTA Button:
**[Verb set by the playbook]**

### Trust Line:
[Short reassurance microcopy — e.g. "No Credit Card Required".]
```

The shipped design labels the name tag "Coach" and the subtext "With an Expert Coach" — both are
banned terms (Brand Core §3). Copy always uses "Teacher".

**When to use which:** Option A is required on paid ad LPs and the homepage, because their CTA starts
Combined Funnel Onboarding — never swap it for Option B there. Option B is for other student pages
where a believable "watch it happen" video or image should lead; the media carries the credibility a
stat trust bar would otherwise supply, which is why Option B has no trust bar or A/B headline. Don't
combine both trust devices on one page. Event pages use the Event Registration Hero (§17) instead.

**Option B's CTA** was read from Figma as a plain button. Figma lagged production on Option A's
form, so verify against a live Option B page before assuming it stays button-only.

---

## 2. LOGO MARK

A lightweight trust strip immediately after the hero — press logos, partner logos, or a secondary
link. Mostly visual; copy needs are minimal.

```
### Eyebrow (optional):
[e.g. "As Featured In" — omit if logos are self-explanatory.]

### Secondary link/CTA (optional):
**[3–5 words, e.g. "Learn More About Our Teachers"]**
```

Logos-only, link-only, or both — use only what the page needs.

---

## 3. BENEFITS GRID SECTION

_Sources: Figma node 10352-78 ("1-on-1 Yoga for Hormonal Balance & Women's Health"); node 10062-5814
("Why Teach With MyYogaTeacher", teacher recruitment); live free event page ("In 45 minutes, you
will")._

```
### Section Headline:
**[e.g. "Personalized Yoga for Your Hormonal Health Needs" / "Why Teach With MyYogaTeacher" /
  "In 45 minutes, you will"] — ~4–9 words / ~20–60 chars.**

### Intro Paragraph or Line:
[Student pages: ONE paragraph, ~30–40 words — name the breadth of the topic, then bridge to
 "your practice should reflect what you need." Recruitment pages: one short line, ~8 words —
 e.g. "You bring the expertise. We handle the rest." Event pages: omit — the headline frames the grid.]

### Grid (6 cards, 2×3 layout):
Card format:
**[Title — 2–5 words]**
[1–2 sentences, ~7–25 words. What this need/benefit/outcome means for the reader.]

### CTA Button (optional — omit on event pages):
**[Verb set by the playbook]**
```

**Event variant:** a headline naming the session length ("In 45 minutes, you will") and 6 outcome
cards — what the attendee will do or learn in the session. Titles 2–5 words; one-line descriptions
~7–12 words. No intro, no CTA.

**When to use:** student pages on broad topics that break into sub-conditions or sub-needs (e.g.
hormonal health → PCOS, PMS, irregular periods, endometriosis & fibroids, fertility-related stress,
overall wellness); teacher hiring pages for the reasons to join. Not redundant with the Benefit
Section: this maps the *breadth*, the Benefit Section makes the case for MYT's approach. Skip on
narrow single-condition pages.

---

## 4. BENEFIT SECTION

_Sources: Figma node 7635-5187 (Prenatal); prenatal teacher recruitment copy doc (specialization
module); live free event page ("This is for you if...")._

```
### Eyebrow (optional):
[2–4 words, e.g. "A Specialized Opportunity"]

### Section Headline:
**[e.g. "Personalized Prenatal Yoga for Every Stage of Your Journey" / "This is for you if..."]
  — ~4–10 words / ~20–60 chars.**

### Intro Paragraph (omit on event pages):
[~40–50 words. Open with the problem/aspiration this page addresses — specific and relatable —
 then land on the MYT solution: personalized, certified, live. May split into two short
 paragraphs.]

### 4 Key Benefits (student pages; omit on recruitment specialization modules):
✓ **[Benefit 1 — primary outcome, ~6–9 words]**
✓ **[Benefit 2 — secondary outcome, ~6–9 words]**
✓ **[Benefit 3 — mental/emotional or related benefit, ~6–9 words]**
✓ **[Benefit 4 — convenience/lifestyle fit, ~6–9 words]**
```

**Event variant ("This is for you if..."):** headline plus 4 audience-fit bullets, ~12–16 words
each, describing the situations of people who should register (e.g. repeat attendees, first-timers,
people who want live guidance instead of videos). No intro, no CTA.

Tone and framing (empathy-first, identity-first, aspirational) come from the playbook; the shape
doesn't change.

---

## 5. HOW IT WORKS

_Source: Figma node 7635-5187 (Prenatal)._

The **ongoing service experience** — what happens once someone is practicing with MYT. Distinct from
Easy to Get Started (§11), which covers the steps to **begin**. A page can carry both.

```
### Section Headline:
**[e.g. "How It Works" / "Your [Topic] Journey in 3 Simple Steps"] — 2–6 words.**

### Step 1: [Title, 2–4 words]
[2 sentences, ~18–22 words. Share your situation/goal → a plan is designed for you.]

### Step 2: [Title, 2–4 words]
[2 sentences, ~18–22 words. What live delivery looks like — guidance, correction, in real time.]

### Step 3: [Title, 2–4 words]
[2 sentences, ~18–22 words. How the practice evolves / the long-term outcome.]
```

Always 3 steps unless a playbook has a structural reason for more.

---

## 6. TEXT TESTIMONIALS

_Source: Figma node 7635-5187 (Prenatal)._

```
### Section Headline:
**[e.g. "What First-Time [Audience] Are Saying" / "Trusted by [Audience]"] — ~6–12 words.**

### Subheadline:
[1 sentence reinforcing empathy/credibility, ~10–15 words.]

### Testimonials (5–6 total):
Format per testimonial:
**[Name]**
[Descriptor, e.g. "MyYogaTeacher Member" — no location needed]
"[2–4 sentence quote, ~40–60 words. Names a specific result, not generic praise.]"
```

**Quality rules:**
- Real quotes first. Anything generated is a clearly marked placeholder.
- No "amazing teacher, highly recommend" — every quote names a concrete result.
- Across the set, include one quote about a failed prior solution and one about emotional/lifestyle
  impact beyond the physical.

---

## 7. EXPERT TEACHERS

_Sources: Figma node 7635-5187 (Prenatal); prenatal teacher recruitment copy doc._

```
### Section Headline:
**[e.g. "Meet Our Prenatal Yoga Experts" / "Meet Our Certified Yoga Teachers"]**

### Subheadline (optional):
[1 sentence on specializations relevant to this page, ~10–20 words.]

### Teacher Cards (3–6):
- Photo
- Name
- Experience/credential line (e.g. "12 years of teaching experience")
- Rating (e.g. "4.9 from [N] reviews") — student pages
- Student quote (optional, 1–2 sentences) — used on recruitment pages

### CTA Button (optional):
**[Verb set by the playbook]**
```

Pages led by a single teacher (e.g. events) use Meet {Teacher} (§18) instead.

---

## 8. COMPARISON TABLE

_Source: Figma node 7635-5187 (Prenatal); paid-LP copy docs._

```
### Section Headline:
**MyYogaTeacher vs. [Comparison frame] — ~6–10 words.**

### Subheadline:
[1 sentence framing the differentiation, ~10–15 words.]

| Feature | MyYogaTeacher | [Alternative] |
|---------|---------------|----------------|
| [Attribute 1] | ✅ [Strength, 4–8 words] | ❌ [Gap/risk, 4–8 words] |
| [Attribute 2] | ✅ [Strength, 4–8 words] | ❌ [Gap/risk, 4–8 words] |
| [Attribute 3 — page-specific] | ✅ [Strength] | ⚠️/❌ [Gap] |
| [Attribute 4 — page-specific] | ✅ [Strength] | ❌ [Gap] |
```

4–6 rows. The comparison frame and page-specific rows come from the playbook.

---

## 9. VIDEO TESTIMONIALS

_Sources: Figma nodes 7635-5187 and 10062-5814._

```
### Section Headline:
**[Thematic — e.g. "See Why Students Love MyYogaTeacher" / "What Our Teachers Are Saying"] — ~5–8 words.**

### Video Cards (3–4):
Thumbnail + play button + name + descriptor (e.g. "MyYogaTeacher Member") + optional short
caption (~5–10 words).

### Rating Strip (optional, if not already shown elsewhere on the page):
- [N]K+ 5-star reviews
- 4.9 App Store rating
```

---

## 10. ELIGIBILITY CHECKLIST

_Source: Figma node 10062-5814 ("What You'll Need", teacher recruitment)._

```
### Section Headline:
**What You'll Need** (or page-appropriate equivalent, 2–4 words)

### Requirements Checklist (5–7 items):
✓ [Requirement, ~4–14 words]
✓ [Requirement, ~4–14 words]
✓ [Requirement, ~4–14 words]
✓ [Requirement, ~4–14 words]
✓ [Requirement, ~4–14 words]

### Closing Note (optional):
[1 sentence, ~12–16 words. A practical heads-up for the application step —
 e.g. "Have your resume and total training hours ready — you'll need both for the application."]
```

**When to use:** recruitment or application pages, and workshops with prerequisites (e.g. TTC).
Skip on student conversion pages.

---

## 11. EASY TO GET STARTED

_Source: Figma node 10062-5814 ("Easy to get started", teacher recruitment)._

The steps to **begin** — sign up, apply, onboard — not the ongoing experience (§5 How It Works).

```
### Section Headline:
**[e.g. "Easy to Get Started" / "Getting Started Is Simple"] — 2–5 words.**

### Step 1: [Title, 2–5 words]
[1–2 sentences, ~18–25 words. What happens in this step.]

### Step 2: [Title, 2–5 words]
[1–2 sentences, ~18–25 words.]

### Step 3: [Title, 2–5 words]
[1–2 sentences, ~18–25 words.]

[3 or more steps — add steps if the flow genuinely has more stages.]

### Closing Tagline (optional):
[1 sentence, ~10–14 words — e.g. "We bring the students and manage the platform — you focus on teaching."]
```

Numbered badges with a connecting vertical line are the usual visual treatment.

---

## 12. FAQ SECTION

_Sources: Figma node 7635-5187; prenatal teacher recruitment copy doc._

```
### Section Headline:
**Frequently Asked Questions** (or "FAQs")

### Subheadline (optional):
[1 short line, ~5–8 words, e.g. "Quick answers to commonly asked questions."]

### FAQs (6–7 total):
Q: [~6–16 words]
A: [1–3 sentences, ~10–45 words]
```

**Coverage** comes from the playbook. Default for student pages: a "does this work for me" question,
beginner reassurance, timeline/results, safety/objection, one page-specific question, and one
logistics/frequency question.

**Medical disclaimer trigger:** if the topic involves pain, a health condition, pregnancy/postpartum,
or mental health, add the Brand Core §6 short-form disclaimer to the relevant answer and flag it for
footer placement.

---

## 13. LANDING CTA

_Sources: Figma node 7635-5187; prenatal teacher recruitment copy doc._

```
### Main Headline:
**[Emotionally resonant or action-forward. Addresses the core tension for this audience.] — ~6–12 words.**

### Subheadline:
[Primary action + 1 outcome-specific reassurance, ~55–140 chars.]

### CTA Button:
**[Same verb as the hero]**

### Trust Line (optional):
[e.g. "No Credit Card Required" / "Trusted by [N]+ teachers across the globe"]
```

---

## 14. WHAT'S INCLUDED ⚠️ Provisional

_No shipped source yet — carried over from the retired event skill's spec. The shipped free event
page covers "what you'll get" with a Benefits Grid event variant instead, so free events don't use
this; kept for multi-session workshops. Recalibrate against the first workshop example._

```
### Section Headline:
**[e.g. "Inside the [Event Name]" / "Your [N]-Day Program at a Glance"] — 3–7 words.**

### Modules / Sessions / Weeks (3–5):
**[Title, 2–5 words]**
[2 sentences: what's covered and what the attendee leaves with.]

### Included Checklist (optional):
✓ [Live sessions / recordings / worksheets / community access / certificate]
```

---

## 15. EVENT DETAILS CARD ⚠️ Provisional

_No shipped source yet — carried over from the retired event skill's spec. The shipped free event
page puts time selection inside the registration form ("Pick a Time"), so it has no details card;
use this only if a workshop or main event reference shows one._

```
| | |
|-|-|
| **Date** | [Date] |
| **Time** | [Time + timezone] |
| **Duration** | [e.g. 60 minutes / 4 weeks] |
| **Format** | [Live via Zoom / Live + replay] |
| **Price** | [Free / amount] |
| **Seats** | [Only if a real limit exists] |
| **What you need** | [e.g. yoga mat, comfortable clothes, no experience required] |

### CTA Button:
**[Registration verb set by the playbook]**
```

---

## 16. PRICING BLOCK ⚠️ Provisional

_No shipped source yet. Minimal structure only — confirm layout and fields against the first paid
workshop example before relying on it._

```
### Section Headline:
**[e.g. "Enroll in [Workshop Name]"] — 3–6 words.**

### Price:
[Amount + currency; payment plan if one exists]

### What's Covered (3–5 bullets):
✓ [Inclusion, ~3–8 words]

### CTA Button:
**[Verb set by the playbook]**

### Reassurance Line (optional):
[Only real policy — e.g. refund terms as confirmed by the user. Never invent.]
```

---

## 17. EVENT REGISTRATION HERO

_Source: live page `myyogateacher.com/events/yoga-for-sciatica`. Figma `Event-Page` node 2-2202
structure check pending._

The hero for event pages. The page's one real action is submitting this registration form — every
other CTA on the page scrolls to it. The form usually sits in the hero; if the user wants it as
section 2, keep the hero's copy elements here and place the form panel (same copy) directly below.

```
### H1 (Main Headline):
**[The session's promise — ~35–45 chars. e.g. "Gentle Yoga Guidance for Sciatica Pain"]**

### Subheadline:
[2 sentences, ~25–35 words: length + format + who leads it, what attendees will do, where they
 join from. e.g. "A 45-minute live session with a certified teacher — slow, beginner-friendly
 movements for your lower back, hips, and hamstrings, with live corrections and modifications.
 Follow along from your mat at home."]

### Feature Items (3, label + sublabel):
- **[Label, 2–3 words]** — [Sublabel, 2–4 words]   e.g. Live on Zoom — Personalized check-in
- **[Label]** — [Sublabel]                          e.g. All levels welcome — Beginner to Advanced
- **[Label]** — [Sublabel]                          e.g. Free Event — No credit card needed
(Cover format, level, and price.)

### Social Proof (2 short stats):
[e.g. "100+ students reported relief" | "4.9 avg"]

### Registration Form Panel:
- Panel heading: **[2–4 words, e.g. "Save your seat"]**
- Panel subtext: [~6–10 words — effort + seat limit, e.g. "Takes 20 seconds · Seats are limited to 20"]
- Form fields — fixed, don't generate (Full Name, Email Address, Phone (For Reminders), Pick a Time)
- Submit button: **[2 words, e.g. "Register Free"]**
- Line below button: [~5–7 words, e.g. "Free · Live on Zoom · Not recorded"]
- Consent note and system states (no session scheduled, load errors) — fixed, don't generate
```

State a seat limit only if it's real.

---

## 18. MEET {TEACHER}

_Source: live page `myyogateacher.com/events/yoga-for-sciatica` ("Meet Your Teacher"). Figma
`Event-Page` node 2-2202 structure check pending (e.g. photo treatment)._

One teacher introduced in depth — for pages led by a single teacher, such as events. Pages showing
several teachers use Expert Teachers (§7).

```
### Section Headline:
**Meet {Teacher}** — e.g. "Meet Your Teacher" or "Meet [Teacher's first name]"

### Teacher Name:
[Full name]

### Bio:
[3 sentences, ~45–55 words: certification/credentials → education/training → years of experience
 and who they've helped, tied to the page topic.]

### Credential Tags (3–5):
[2–3 words each — e.g. "AYUSH Certified", "200+ Hours TTC", "Yoga Therapy", "YCB Level 3"]
```

No CTA on the shipped page. Credentials and experience must be real — ask for them, never invent.

---

## OPTIONAL / SUPPLEMENTARY COMPONENTS

Available to any page on top of a playbook's recipe.

### Use Cases

```
### Section Headline:
**How You Can Use Our 1-on-1 Sessions** (or page-appropriate equivalent)
⚠️ Design template may read "Coaching" — use "Sessions" in copy per brand rules.

### Cards (2–3):
**[Use Case Title]**
[2-sentence description of who this is for and the outcome.]
🗓 [Frequency tag — e.g., "1–4 sessions/month"]
```

### Testimonials — Alternate Format

```
Component dimensions: 1550×364px. Layout: 2-column card grid.

Card format (per card):
"[Testimonial text — bold/highlight the single most impactful phrase.]
[Name], [Age]"

Generate 2 cards, complementing (not replacing) the main Text Testimonials section.
```

### For Your Unique Needs

```
### Section Headline:
**For Your Unique Needs**

### 6 Image Cards (2×3 grid):
Each card = a question-framed pain point as overlay text on a lifestyle image.
Format: "[Relatable situation]?" (e.g., "Desk work causing aches and pains?")
```

Best for broad pages serving multiple sub-audiences or pain points.
