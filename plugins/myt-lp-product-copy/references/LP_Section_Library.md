# MYT Landing Page — Section Library

Shared, reusable templates for every section/component used across MyYogaTeacher landing
pages. These are **not** owned by any one LP category (paid ads, events, teacher hiring,
product). Every LP-generating skill picks, sequences, and lightly adapts (tone, CTA
vocabulary, funnel goal) from this library rather than each holding its own copy — that
duplication is exactly the brand-drift problem this plugin exists to prevent.

**Out of scope for this library:** the site navigation bar and footer. Both are fixed across
every page and are never regenerated as copy.

Word/character counts below are calibrated against a real shipped MYT LP (Figma:
`Branding-page-updates`, Prenatal page) — treat them as realistic targets, not hard caps.

---

## Standard Sequence

1. Hero Section _(two coequal options: Combined Funnel Header, or Media Hero Section)_
2. Logo Mark
3. Benefits Grid Section _(conditional — only when the topic has multiple sub-conditions/needs)_
4. Benefit Section
5. How It Works
6. Text Testimonials
7. Expert Teachers
8. Comparison Table
9. Video Testimonials
10. Eligibility Checklist _(conditional — recruitment/application pages only)_
11. Easy to Get Started _(conditional — onboarding/application-flow pages)_
12. FAQ Section
13. Landing CTA

A generating skill may reorder, drop, or repeat sections (e.g., an event LP may swap
Comparison Table for an Event Details card) but should default to this order unless the page
goal calls for a different flow.

---

## 1. HERO SECTION

Two named alternatives for the same slot (section 1) — pick one per page, not both. They're
coequal choices, not a primary/fallback pair: which one to use depends on whether the page's
strongest asset is aggregate social proof or a compelling piece of media.

### Option A — Combined Funnel Header

Built around stat-based trust signals (ratings, press) — and, critically, an **inline lead
capture form**, not just a plain CTA button. This is the actual live production hero used
across all paid landing pages; the dev-mode Figma frames checked earlier hadn't been updated
to reflect it, so the form was missing from this library until now.

```
### H1 (Main Headline):
**[Keyword/benefit-led. ~40–45 chars. Names the topic/program and the core promise. e.g.
  "1-on-1 Online Yoga Classes for Flexibility"]**

### H1 (Alternative for A/B Testing):
**[Word-order variant or identity/outcome reframe. Different structure from primary H1.]**

### Subheadline:
[Benefit-led expansion, ~50–60 chars. e.g. "Build Flexibility and Strength with Personalized Yoga"]

### Lead Capture Form (inline in hero — the CTA lives here, not as a standalone button):
- Name field — placeholder text: "Your name"
- Phone field — country-code selector (flag + dial code dropdown) + placeholder text:
  "Your WhatsApp number"
- Submit button (this IS the primary CTA): **[Action verb matched to the funnel goal — e.g.
  "Book a Free Session" / "Register Now" / "Apply Now". Set by the calling skill.]**

### Trust Line:
[Directly beneath the form — e.g. "No Credit Card Required" / "Limited Spots Available".]

### Trust Bar (2–3 stat items, laurel/badge style):
- [N]K+ 5 star ratings
- 4.9 App Store
- [optional third — e.g. press mention]

### Hero Visual:
[Full-bleed lifestyle/mood photo background — person, setting, expression, pose. No text baked
 into the image; H1/subheadline/form render on top of it.]
```

**Form field copy stays fixed** ("Your name" / "Your WhatsApp number") — only the submit
button's verb changes per funnel goal, same as the CTA verb did before.

### Option B — Media Hero Section

_Calibrated against a third shipped MYT LP (Figma: `Branding-page-updates`, node 5006-944 —
"Back Pain - V1 - No video")._

Built around showcasing media — the visual isn't decoration here, it's the section's main
trust-building device, so it's the first field, not the last.

```
### Hero Visual — Video or Image (required, defines this option):
[A live-session preview, not a generic lifestyle photo: framed like an in-progress Zoom call.
 Include a "LIVE" badge, an in-call control bar (mute/camera-style icons), and a name tag
 identifying the teacher (e.g. "Coach"). Works as a static image or an actual video loop —
 the surrounding copy is identical either way.]

### H1 (Main Headline):
**[Keyword/benefit-led. ~30–40 chars — shorter than Option A since there's no A/B alt to
  balance against. e.g. "1-on-1 Yoga At Home for Back Pain"]**

### Subtext:
[One short line, ~5–7 words / ~30–40 chars, naming the format — e.g. "With an Expert Coach,
 Live via Zoom".]

### Primary CTA Button:
**[Action verb matched to the funnel goal]**

### Trust Line:
[Short reassurance microcopy — e.g. "No Credit Card Required".]
```

**When to use which:** Option A when the page needs aggregate social proof (ratings, press) to
build trust fast and doesn't have a strong visual asset to lead with. Option B when there's a
believable "watch it happen" video or image — the media carries the credibility that the stat
trust bar would otherwise supply, which is why Option B doesn't also carry a trust bar or an
A/B headline. Don't combine both trust-building devices on one page.

**Note on Option B's CTA:** confirmed from a Figma dev-mode frame as a plain button (no inline
form). Given Option A's form was missing from that same Figma file until corrected against a
live production screenshot, verify against the live page before assuming Option B stays
button-only — Figma here has lagged production before.

**Adaptation note:** for Option A, the submit-button verb, trust line, and whether pricing
appears here are the only things that change per page goal — the form fields themselves don't.
For Option B, the CTA verb and trust line are what change. The rest of whichever option is
chosen stays fixed.

---

## 2. LOGO MARK

A lightweight trust strip that runs immediately after the header — press logos, partner
logos, or a secondary link. Mostly a visual asset; copy needs are minimal.

```
### Eyebrow (optional):
[e.g. "As Featured In" — omit if logos are self-explanatory.]

### Secondary link/CTA (optional):
**[3–5 words, e.g. "Learn More About Our Teachers"]**
```

Use only what the page needs — this section can be logos-only, link-only, or both.

---

## 3. BENEFITS GRID SECTION

_Calibrated against a second shipped MYT LP (Figma: `Branding-page-updates`, node 10352-78 —
"1-on-1 Yoga for Hormonal Balance & Women's Health"). Sits right after Logo Mark, ahead of the
Benefit Section._

```
### Section Headline:
**[Personalized [Topic] for Your [Need/Goal]] — ~7–9 words / ~50–60 chars.**

### Intro Paragraph:
[ONE paragraph, ~30–40 words. Name the breadth of the topic — how it shows up differently for
 different people — then bridge to "your practice should reflect what you need."]

### Needs Grid (6 cards, 2×3 layout):
Card format:
**[Sub-condition / Sub-need Title — 2–4 words]**
[1 sentence, ~10–15 words. What the practice offers for this specific need.]

### CTA Button:
**[Matched to funnel goal — e.g. "Book a Free Session"]**
```

**When to use:** best for broad topics that naturally break into multiple sub-conditions or
sub-needs (e.g. hormonal health → PCOS & hormonal imbalance, PMS & painful periods, irregular
periods, endometriosis & fibroids, fertility-related stress, overall hormonal wellness). This
section isn't redundant with the Benefit Section that follows it: this one maps the *breadth*
of the topic (which specific need brought this visitor here), the Benefit Section makes the
case for MYT's approach generally. Skip entirely on narrower, single-condition pages.

Also confirmed on a teacher-recruitment page (node 10062-5814) as "Why Teach With
MyYogaTeacher" — same headline+intro+6-card-grid shape, reused for recruitment reasons-to-join
instead of student sub-conditions. Further evidence this section belongs to the shared library,
not to paid student-facing LPs specifically.

---

## 4. BENEFIT SECTION

_(Previously "How MYT Can Help" — same template, category-neutral name.)_

```
### Section Headline:
**[Personalized [Topic] for [Goal/Stage/Outcome]] — ~8–10 words / ~60 chars.**

### Intro Paragraph:
[ONE paragraph, ~40–50 words. Open with the problem/aspiration this page addresses —
 specific and relatable — then land on the MYT solution: personalized, certified, live.]

### 4 Key Benefits:
✓ **[Benefit 1 — primary outcome, ~6–9 words]**
✓ **[Benefit 2 — secondary outcome, ~6–9 words]**
✓ **[Benefit 3 — mental/emotional or related benefit, ~6–9 words]**
✓ **[Benefit 4 — convenience/lifestyle fit, ~6–9 words]**
```

**Adaptation note:** tone shifts by audience (empathy-first for condition/pain topics,
identity-first for audience-specific pages, aspirational for style/lifestyle pages) — the
calling skill sets this; the section shape doesn't change.

---

## 5. HOW IT WORKS

Describes the **ongoing service experience** — what happens once someone is practicing/
engaged with MYT (the session/practice journey). Distinct from Easy to Get Started (below),
which describes the **onboarding/application process** to begin in the first place. A page can
carry both as separate sections when it needs to show both.

```
### Section Headline:
**[e.g. "How It Works" / "Your [Topic] Journey in 3 Simple Steps"] — 2–6 words.**

### Step 1: [Title, 2–4 words]
[2 sentences, ~18–22 words. Share your situation/goal → a plan is designed for you.]

### Step 2: [Title, 2–4 words]
[2 sentences, ~18–22 words. What live delivery looks like — guidance, correction, real-time.]

### Step 3: [Title, 2–4 words]
[2 sentences, ~18–22 words. How the practice evolves / the long-term outcome.]
```

Always 3 steps unless the calling skill has a structural reason for more (e.g. a multi-week
program breakdown), in which case treat it as a variant, not a redefinition of this template.

---

## 6. TEXT TESTIMONIALS

```
### Section Headline:
**[e.g. "What First-Time [Audience] Are Saying" / "Trusted by [Audience]"] — ~8–12 words.**

### Subheadline:
[1 sentence reinforcing empathy/credibility, ~10–15 words.]

### Testimonials (5–6 total):
Format per testimonial:
**[Name]**
[Descriptor, e.g. "MyYogaTeacher Member" — no location needed]
"[2–4 sentence quote, ~40–60 words. Names a specific result, not generic praise.]"
```

**Quality rules:**
- No "amazing instructor, highly recommend" — every quote names a specific, concrete result.
- Across the set, include at least one quote referencing a failed prior solution and one
  referencing emotional/lifestyle impact beyond the physical.

---

## 7. EXPERT TEACHERS

_(Previously "Expert Showcase" — same template, category-neutral name.)_

```
### Section Headline:
**Meet Our [Topic] Experts / Meet Our Certified Yoga Teachers**

### Subheadline:
[1 sentence on relevant specializations for this page, ~10–15 words.]

### Teacher Cards (3–4):
- Photo
- Name
- Certifications (e.g., "500-Hour RYT, [Relevant Specialty]")
- Review count/rating (e.g., "4.9 ★ from [N]+ students")
- Specializations (2–3 relevant tags)

### CTA Button:
**[Matched to funnel goal — e.g. "Start Your Free Trial"]**
```

---

## 8. COMPARISON TABLE

```
### Section Headline:
**MyYogaTeacher vs. [Confirmed comparison frame] — ~8–10 words.**

### Subheadline:
[1 sentence framing the differentiation, ~10–15 words.]

| Feature | MyYogaTeacher | [Alternative] |
|---------|---------------|----------------|
| [Attribute 1] | ✅ [Strength, 4–8 words] | ❌ [Gap/risk, 4–8 words] |
| [Attribute 2] | ✅ [Strength, 4–8 words] | ❌ [Gap/risk, 4–8 words] |
| [Attribute 3 — page-specific] | ✅ [Strength] | ⚠️/❌ [Gap] |
| [Attribute 4 — page-specific] | ✅ [Strength] | ❌ [Gap] |
```

4–6 rows total. The comparison frame (who/what MYT is being compared against) is set by the
calling skill per page — the row structure itself doesn't change.

---

## 9. VIDEO TESTIMONIALS

```
### Section Headline:
**[Thematic — e.g. "Real People, Real Results/Transformations"] — ~5–8 words.**

### Video Cards (3–4):
Thumbnail + play button + name + short caption overlay (~5–10 words per caption).

### Rating Strip (optional, if not already shown elsewhere on the page):
- [N]K+ 5-star reviews
- 4.9 App Store rating
```

---

## 10. ELIGIBILITY CHECKLIST

_New from a teacher-recruitment page (Figma: `Branding-page-updates`, node 10062-5814 — "What
You'll Need"). Application/recruitment pages only — not applicable to student-facing
conversion LPs._

```
### Section Headline:
**What You'll Need** (or page-appropriate equivalent, 2–4 words)

### Requirements Checklist (5–7 items):
✓ [Requirement 1, ~8–14 words]
✓ [Requirement 2, ~8–14 words]
✓ [Requirement 3, ~8–14 words]
✓ [Requirement 4, ~8–14 words]
✓ [Requirement 5, ~8–14 words]

### Closing Note (optional):
[1 sentence, ~12–16 words. A practical heads-up for the application step —
 e.g. "Have your resume and total training hours ready — you'll need both for the application."]
```

**When to use:** recruitment/application-type pages (teacher hiring, partner/affiliate
programs) where eligibility criteria need to be stated upfront, before the applicant commits
time to applying. Skip on student-facing conversion LPs and events.

---

## 11. EASY TO GET STARTED

_New from the same teacher-recruitment page (node 10062-5814 — "Easy to get started"). Not a
duplicate of How It Works — see the distinction noted there: this section describes the steps
to **begin** (sign up, apply, onboard), not the ongoing experience once begun._

```
### Section Headline:
**[e.g. "Easy to Get Started" / "Getting Started Is Simple"] — 2–5 words.**

### Step 1: [Title, 2–5 words]
[1–2 sentences, ~18–25 words. What happens in this step of signing up/applying.]

### Step 2: [Title, 2–5 words]
[1–2 sentences, ~18–25 words.]

### Step 3: [Title, 2–5 words]
[1–2 sentences, ~18–25 words.]

[Repeat for additional steps — 3 or more, unlike How It Works this isn't capped at 3 —
 if the onboarding/application flow genuinely has more stages.]

### Closing Tagline (optional):
[1 sentence, ~10–14 words. A reassurance/summary line beneath the steps —
 e.g. "We bring the students and manage the platform — you focus on teaching."]
```

Numbered badges (1./2./3.) with a connecting vertical line are a common visual treatment for
this section. **When to use:** any page where the friction being addressed is "how do I
actually begin" — recruitment/application flows most often, but also usable on a conversion LP
that wants to walk through the sign-up steps (book → match with a teacher → start practicing)
separately from how the practice itself works.

---

## 12. FAQ SECTION

```
### Section Headline:
**Frequently Asked Questions**

### Subheadline:
[1 short line, ~5–8 words, e.g. "Quick answers to commonly asked questions."]

### FAQs (6–7 total):
Q: [~8–16 words]
A: [2–3 sentences, ~30–45 words]
```

**Recommended coverage** (adapt per page, don't treat as rigid slots): a validating "does this
work for me" question, a beginner-reassurance question, a timeline/results question, a
safety/objection question, one page-specific question, and one logistics/frequency question.

**Medical disclaimer trigger:** if the page topic involves pain, a health condition,
pregnancy/postpartum, or mental health — add a disclaimer note to the relevant FAQ answer and
flag it for footer placement. This is a per-topic adaptation, not part of every FAQ instance.

---

## 13. LANDING CTA

```
### Main Headline:
**[Emotionally resonant or action-forward. Addresses the core tension for this audience.] — ~8–12 words.**

### Subheadline:
[Primary action + 1 outcome-specific reassurance, ~55–120 chars.]

### CTA Button:
**[Matched to funnel goal]**

### Trust Line (optional):
[Context-appropriate — e.g. "No Credit Card Required" / "Limited to X Spots"]
```

---

## OPTIONAL / SUPPLEMENTARY COMPONENTS

These are available to any page, on top of the standard sequence — not tied to any LP
category.

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

Best for broad pages serving multiple sub-audiences or multiple pain points.

---

## Explicitly excluded from this library

- **Navigation bar** — fixed sitewide, not regenerated per page.
- **Footer** — fixed sitewide, not regenerated per page.
- **"Recent bookings" live activity strip** (real-time names/times/ratings) — a dynamic,
  data-driven widget, not static copy. Out of scope for copy generation.
