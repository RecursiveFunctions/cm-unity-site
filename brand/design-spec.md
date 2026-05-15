---
title: "CMUnity — Brand & Web Design Specification"
subtitle: "A brief for the brand designer"
author: "CMUnity"
date: "May 2026"
version: "v1.0"
---

# CMUnity — Brand & Web Design Spec

**Purpose.** This document briefs a designer on the visual identity work needed to bring CMUnity to a finished, official-org standard: typography, logo system (logo, mark, wordmark, favicon), color, and a refreshed site template.

**Status.** CMUnity is an official Carnegie Mellon student organization (effective 2026). The current site (`cm-unity.org`) is a holding page built in Tailwind with CMU's red and a borrowed editorial type pairing. It establishes mood but is not a finished identity.

**Point of contact.** rsunadaw@andrew.cmu.edu (org), rfernan2@andrew.cmu.edu (web).

**Live site:** [cm-unity.org](https://cm-unity.org) · **Repo:** github.com/recursivefunctions (Jekyll on GitHub Pages) · **Socials:** instagram.com/cm.unity · discord.gg/ECMDdHva

---

## 1. About CMUnity

CMUnity is a student-led organization at Carnegie Mellon University that exists to:

- **Break cliques and heal polarization** by hosting structured discussion and debate across student groups.
- **Advocate for mental health** and the structural conditions that support student wellbeing.
- **Champion interdisciplinary, self-motivated learning** — curiosity beyond a major's requirements.
- **Foreground ethics** in technical and professional life, over pure career optimization.

Programming includes weekly general-body meetings, facilitated discussions on policy / religion / disparities, and the **Debates** series — an archive of inter-org political debates (e.g., CMU Democrats vs. CMU Republicans, YAL vs. CMU Republicans on Venezuela).

**Audience.** Carnegie Mellon undergraduates and graduate students. Secondary: faculty, advisors, prospective members, peer student orgs, and the broader Pittsburgh civic community.

**Brand promise.** *More than just a connection.* CMUnity hosts the conversations the rest of campus skips — seriously, generously, and in public.

---

## 2. Brand positioning & tone

### Voice attributes

CMUnity sounds **serious, civic, and deliberative**. Editorial in posture; humane in execution. The brand should feel like a small institution that takes its students' inner lives seriously — closer to a campus journal of record than to a club promo.

| We are                          | We are not                                |
| ------------------------------- | ----------------------------------------- |
| Considered, deliberate          | Hot-take, performative                    |
| Generous, inviting              | Cliquey, gatekept                         |
| Plural, even-handed             | Partisan-coded                            |
| Editorial, considered typography| Marketing-y, decorative                   |
| CMU-adjacent, recognizable      | A CMU sub-brand pretending to be official |
| Pittsburgh-rooted               | Generic / placeless                       |

### Relationship to CMU's identity

**Hybrid — distinct mark, CMU accents.** CMUnity needs its own mark, wordmark, and primary palette. **CMU red (#C41230) is preserved as a secondary accent only** — used for institutional connection and for moments of emphasis, not as the dominant brand color. The designer should consult CMU's brand guidelines for official student organizations and ensure all marks comply (no co-opting CMU's wordmark, shield, or tartan in a way that suggests official CMU endorsement beyond org-recognition).

### Reference moodboard (for direction only — not to copy)

- **The Atlantic, Lapham's Quarterly, n+1, Comment Magazine** — editorial bones, restrained palettes, serif headlines.
- **Princeton's University Center for Human Values, Stanford's McCoy Family Center for Ethics in Society** — institutional civic seriousness applied to a student-adjacent program.
- **The Markup, The Pudding, Pew Research** — civic / data design; rigorous and modern without being austere.

Avoid: club-marketing aesthetics (loud gradients, sticker packs, dense emoji), generic SaaS landing pages, anything that would read as a startup pitch.

---

## 3. Typography

Type is the single most important brand asset for CMUnity. The current pairing (Playfair Display + Open Sans) is close in spirit but needs to be reconsidered as a system — heading, body, accent — with deliberate scale, weights, and a brand-defining display face.

### What we need

| Role               | Function                                                                                          |
| ------------------ | ------------------------------------------------------------------------------------------------- |
| **Display serif**  | Headlines, hero, marquee debate titles. Should carry editorial weight and a recognizable voice.   |
| **Body sans**      | Long-form reading, UI, captions. Neutral, legible across sizes, with good italics and small caps. |
| **Accent / mono**  | Citation, byline, dateline, debate metadata, data labels. Adds civic-document texture.            |

### Direction for the designer

- Propose **2–3 candidate pairings**. At least one option should use **open-licensed faces** (Google Fonts / SIL OFL) so the site can ship without commercial licensing; at least one may include a commercial face if it materially strengthens the brand.
- Display serif should feel like a *journal*, not a *wedding invitation*. Candidates to consider: **Source Serif 4, Newsreader, Fraunces (with care), GT Sectra, Tiempos Headline, Publico Headline, Lyon Display, EB Garamond, Caslon Doric Display**. Avoid Playfair Display (overexposed).
- Body sans should be **functional and warm** — neither stiff nor playful. Candidates: **Inter, Söhne, Untitled Sans, IBM Plex Sans, GT America, ABC Diatype, Source Sans 3**.
- Accent mono is optional but encouraged: **JetBrains Mono, IBM Plex Mono, GT America Mono, Berkeley Mono**.

### Deliverables (typography)

- Final pairing recommendation with rationale.
- A complete **type scale** (display, h1–h6, body large, body, small, caption) with sizes, line-heights, and tracking for both web (rem-based) and print.
- Weight and style usage rules (when to italicize, when to use small caps, when to use the mono).
- **Webfont licensing path** and CSS `@font-face` strategy.
- A **fallback stack** for each role.

---

## 4. Color

### Direction

CMUnity's palette should feel **deliberative and rooted** — not neutral-corporate, not student-club bright. Think a single confident primary, a deep neutral, warm paper-like grounds, and CMU red held back for accent.

### Recommended composition (designer may adjust)

- **One primary brand color** (not red). A considered, slightly desaturated hue with editorial weight — e.g., a deep ink, oxblood, forest, slate, or indigo. This is the dominant color of the site and identity.
- **One neutral / surface family** — a warm off-white "paper" plus 3–5 grays (warm, not cool) for typography and UI surfaces.
- **CMU red (#C41230) as a reserved accent** — used sparingly for institutional moments (CTA hover, "Carnegie Mellon" attribution, an underline beneath the wordmark on official-org headers). Should never carry the bulk of a page.
- **Two functional accents** — for the Debates series, where we already use two-color framing to represent opposing positions. These should be brand-tuned versions of "voice A / voice B" colors (the current site uses ad-hoc blue / yellow / red — the designer should formalize this).

### Deliverables (color)

- Final palette with **named tokens** (e.g., `ink`, `paper`, `accent-cmu`, `voice-a`, `voice-b`, `mute-1…5`).
- For each color: **hex, RGB, HSL, CMYK, Pantone (nearest), and CSS custom-property name**.
- A **WCAG AA contrast matrix** showing every text-on-surface combination the site uses, with pass/fail notation. Brand should hit AA for body and AAA for body where feasible.
- A **dark-mode variant** of the palette (CMUnity hosts long-form reading; dark mode matters).

---

## 5. Logo system

CMUnity needs a full logo system, not a single asset. The current site uses a placeholder "C" in a black disc — this should be replaced.

### System overview

| Asset            | Use                                                                                    |
| ---------------- | -------------------------------------------------------------------------------------- |
| **Primary lockup** (mark + wordmark) | Default brand presentation — site header, social profile banners, email signatures, presentation title slides. |
| **Mark only**    | Tight contexts where the wordmark is illegible — favicon, app icon, social avatars, t-shirt embroidery, watermarks. |
| **Wordmark only**| Type-led contexts — page footers, document letterheads, print headers where a mark would feel cluttered. |
| **Inverse / single-color variants** | Reversed for dark backgrounds; one-color for monochrome print, embroidery, and small-format use. |

### Mark concept direction

The mark should evoke **connection / bridges** *and* **unity / circle / gathering** — these are the two ideas that most directly translate the org's mission ("more than just a connection," healing polarization, breaking cliques).

Concept seeds for the designer to explore:

1. **Bridged circle.** A circular form interrupted and rejoined by a horizontal element — gap + bridge. Reads as both a gathering (the ring) and a connection across difference (the bridge).
2. **Two arcs meeting.** Two open semicircles inclined toward each other, forming a complete circle only when read together. Evokes dialogue and consent.
3. **Woven node.** Several lines crossing through a single point or knot — gathering, weaving, common ground. (Carries a subtle tartan/weave echo to CMU without literal plaid.)
4. **Concentric gathering.** Rings of varying weight radiating from / pulling toward a center — community formation.

The designer should produce explorations across all four directions before narrowing. The final mark must:

- Read at **16×16 px** (favicon) without losing identity.
- Work as a **single-color silhouette** on red, white, black, and the brand primary.
- Survive **embroidery and screen-print** reproduction (no hairline strokes, no gradients in primary use).
- Avoid resemblance to CMU's official shield, plaid pattern, or "CMU" wordmark.

### Wordmark direction

- "CMUnity" set in a custom or carefully selected display cut. The visual joke — *CMU* nested inside *Community* — should be **typographically articulated**, not literally drawn: e.g., a hairline weight shift, a tonal shift in the "CMU" letters, a small-caps treatment, or a custom ligature. Subtle is better than literal.
- A **secondary descriptor lockup** is required: `CMUnity` over `Carnegie Mellon University` (or `at Carnegie Mellon`) in small caps, to make the institutional affiliation legible at first glance. This descriptor uses the body sans, not the display serif.

### Deliverables (logo)

- Primary lockup, mark, wordmark, and descriptor lockup — each in **full color, single-color black, single-color white, and CMU-red accent variants**.
- File formats: **SVG (primary), PDF, EPS, PNG @ 1x / 2x / 3x, ICO** for favicon.
- A **construction sheet** with grid, proportions, optical adjustments noted.
- **Clear-space and minimum-size rules** for each asset.
- **Misuse examples** (do/don't grid): stretching, recoloring outside palette, placing on insufficient-contrast backgrounds, rotating, adding effects, swapping wordmark fonts.

---

## 6. Favicon

- **Source asset:** the mark, simplified for 16×16 / 32×32 / 48×48 raster delivery.
- **Required outputs:**
  - `favicon.ico` (multi-resolution: 16, 32, 48)
  - `favicon.svg` (modern browsers; respects `prefers-color-scheme` if feasible)
  - `apple-touch-icon.png` (180×180)
  - `icon-192.png`, `icon-512.png` (PWA / Android)
  - `safari-pinned-tab.svg` (single-color)
- **Background-aware variant** for browser dark UI strongly preferred.

---

## 7. Site template

The site is built on **Jekyll + Tailwind CDN** and deployed via GitHub Pages with a custom domain. The designer is **not expected to ship code** — but the deliverable should be Figma/Sketch artwork that a developer can implement in Tailwind without translation guesswork.

### Page templates to design

| Template                | Status      | Notes                                                                                 |
| ----------------------- | ----------- | ------------------------------------------------------------------------------------- |
| **Home (`/`)**          | Refresh     | Hero, mission strip, principles grid (8 values), events module, CTA, footer.          |
| **Debates index (`/debates/`)** | Refresh | Archive grid; each card shows series, year, participating orgs, topic tags, summary.  |
| **Debate detail**       | Refresh     | Long-form: title, participants, date, embedded video, summary, full transcript.       |
| **About / Get involved**| New         | Mission, principles in depth, leadership, meeting cadence, how to join, contact.      |
| **Events**              | New         | Upcoming + past events with date, location, RSVP / Discord link.                      |
| **Writing / dispatches**| Optional    | If we publish op-eds, debate recaps, member essays — a simple article template.       |
| **404**                 | New         | A short, on-brand fallback page.                                                      |

### Layout system

- **12-column grid**, 1280 px max content width, generous outer margins on large screens.
- **Spacing scale:** 4 / 8 / 12 / 16 / 24 / 32 / 48 / 64 / 96 / 128 (px). Designer may extend, not contract.
- **Responsive breakpoints** to mirror Tailwind defaults: `sm` 640, `md` 768, `lg` 1024, `xl` 1280, `2xl` 1536.
- **Reading-width column** for long-form debate transcripts and dispatches: ~68ch.

### Components

The designer should produce a small component library so a developer can implement consistently. At minimum:

- Top navigation bar (desktop + mobile drawer)
- Footer (with socials, attribution, contact, optional newsletter)
- Hero block (with and without supporting image)
- Section heading (eyebrow + headline + lede)
- Principle / value card (the 8-card grid currently in use)
- Event card (date chip, title, location, CTA)
- Debate index card (org-vs-org framing — uses the two "voice" accent colors)
- Debate detail header (participants, date, tags, video embed slot)
- Long-form article body (headings, blockquotes, pull quotes, lists, footnotes, image with caption)
- Buttons (primary, secondary, tertiary / text-link, with states: default, hover, focus, disabled)
- Form controls (input, textarea, select, checkbox — for any future RSVP / signup)
- Tag / pill (used for topic categorization)
- Embedded video container (16:9, with caption and source attribution)

### Motion & interaction

- **Restraint.** No parallax, no scroll-jacking, no aggressive entrance animations. The brand is deliberative; motion should be functional.
- **Acceptable:** subtle hover lifts (≤2 px translate, ≤120 ms ease), underline reveals on links, focus rings (visible, accessible), gentle fade-ins on first scroll-into-view (≤300 ms, no stagger longer than 80 ms).
- **Reduced-motion:** all motion must respect `prefers-reduced-motion: reduce`.

### Accessibility (non-negotiable)

- WCAG **2.1 AA minimum** for color contrast and interactive components.
- Focus states visible on every interactive element.
- Semantic HTML in component specs (`<nav>`, `<main>`, `<article>`, `<header>`, `<footer>`, headings in order).
- Keyboard-navigable from end to end.
- Alt-text guidance and a content authoring note for any future contributors.

### Imagery & iconography

- **Photography direction.** Documentary, available-light, candid — debates in progress, conversations between students, hands taking notes, audience listening. Avoid posed group photos and stock imagery. When stock is unavoidable, prefer Unsplash editorial-style over corporate imagery.
- **Iconography.** The current site uses Font Awesome + emoji. Replace with a **single icon system** — designer to propose (Phosphor, Lucide, or a small bespoke set). One stroke weight, one corner treatment, one optical size system.

---

## 8. Voice & copy guidelines

A short note for the designer (and for whoever writes microcopy on the site):

- **Headlines** are declarative, not promotional. "Bridging campus divides" beats "Join the most inclusive community at CMU!"
- **Subheads and body** are written in plain, civic English. No jargon, no MBA voice, no "synergies."
- **CTAs** are specific. "Join our Discord" beats "Get started." "Read the transcript" beats "Learn more."
- **Attribution.** Carnegie Mellon University is named, never abbreviated, in legal/footer contexts. In running prose, "CMU" is fine.

---

## 9. Deliverables checklist

The designer should return:

**Brand book (PDF, ~20–30 pages)** containing:

- [ ] Mission statement and positioning summary
- [ ] Voice attributes and do/don't
- [ ] Typography: pairing recommendation, type scale, usage rules, fallbacks, licensing
- [ ] Color: full palette with tokens, all color-space values, contrast matrix, dark-mode variant
- [ ] Logo system: lockups, mark, wordmark, descriptor lockup, construction, clear-space, minimum sizes, misuse
- [ ] Favicon strategy and outputs
- [ ] Iconography system selection and usage
- [ ] Photography direction with reference images
- [ ] Site template designs (all pages above) at desktop, tablet, and mobile widths
- [ ] Component library (Figma file)

**Production assets** in a versioned directory (`/brand/v1/`) committed to the repo:

- [ ] All logo lockups in SVG, PDF, EPS, PNG @ 1x/2x/3x
- [ ] All favicon outputs (`.ico`, `.svg`, `.png` at required sizes)
- [ ] Font files (if open-license) or licensing documentation (if commercial)
- [ ] Color tokens as a JSON file *and* a CSS custom-properties file
- [ ] A README explaining how to use the assets and where each lives

**Figma source file** with components, styles, and tokens, shared with the org email.

---

## 10. Constraints

- **Licensing.** Typefaces must be licensable for the org's anticipated use (web + print + apparel). If a commercial face is chosen, the designer should quote the license tier and renewal cadence.
- **CMU brand compliance.** All marks and uses must comply with CMU's official-org brand guidance. CMU's shield, official wordmark, and tartan pattern may not be used directly.
- **Web implementation budget.** The site is Jekyll on GitHub Pages, currently built with Tailwind CDN. The implementation that follows this design work should remain implementable in Tailwind without a JS framework. Avoid designs that require runtime-heavy components (custom WebGL, scroll-stitching, etc.).
- **Accessibility.** AA minimum; the org publicly advocates for mental health and student wellbeing, and an inaccessible site would contradict the brand.

---

## 11. Timeline (placeholder — to be set with designer)

| Phase                         | Duration       | Deliverable                                       |
| ----------------------------- | -------------- | ------------------------------------------------- |
| 1. Discovery & moodboarding   | 1 week         | 3 directional moodboards, narrowed to one         |
| 2. Identity exploration       | 2 weeks        | Logo, mark, wordmark explorations + typography    |
| 3. Identity refinement        | 1 week         | Final identity system + favicon                   |
| 4. Site template design       | 2 weeks        | All page templates at three breakpoints           |
| 5. Component library          | 1 week         | Figma library, tokens, handoff documentation      |
| 6. Production handoff         | 0.5 week       | All production assets in repo + brand book PDF    |

---

## 12. Appendix — current state references

**Current site files (for context only — none are final brand assets):**

- `index.html` — current home page; uses CMU red `#C41230`, Playfair Display, Open Sans, Font Awesome icons, emoji in principle cards.
- `debates/debates.html` — debates index; uses Inter, dark glass-card UI, blue/yellow accents for opposing-voice framing.
- `debates/dems-vs-repubs-25.html`, `debates/venezuela.html` — debate detail pages.

**Open questions to resolve in discovery:**

- Should the wordmark fully spell "CMUnity" or treat "CMU + nity" as two typographic tones?
- Is there appetite for an institutional **secondary mark** (e.g., a seal-style mark for letterheads and certificates) in addition to the primary mark?
- Should the brand support a **publication sub-identity** (the Debates series) — a sibling logotype, or stay unified under one brand?
- Does the org want a **tagline** locked at v1, or kept fluid? Current candidate: *More than just a connection.*

---

*End of brief.*
