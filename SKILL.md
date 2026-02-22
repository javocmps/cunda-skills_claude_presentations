---
name: cunda-presentations
description: |
  Presentation design system for Cunda SpA. Use this skill ONLY when creating PowerPoint presentations, slide decks, or proposal documents for Cunda.

  CRITICAL: Cunda presentations use warm light backgrounds only. NEVER use dark backgrounds — dark colors are for TEXT, not backgrounds.

  Triggers: "presentation", "slides", "deck", "pptx", "propuesta", "pitch deck" combined with "Cunda"
---

# Cunda Presentation Design System

Use these parameters to compose slides freely. The goal is brand coherence and impact — not identical layouts. Each deck should feel unmistakably like Cunda, but tailored to its content and audience.

---

## About Cunda

**Company**: Cunda SpA
**Tagline**: "Empowering to Achieve the Extraordinary"
**Industry**: AI & Software Innovation
**Location**: Santiago, Chile
**Purpose**: To empower people and organizations to achieve the extraordinary.
**What We Do**: Innovation firm that uses AI to help companies transform. We teach, design, and build intelligent agents and custom software that eliminate repetitive tasks, analyze data, and free up resources.
**Recognition**: Selected by Microsoft for Startups and Mana Tech.

---

## Voice & Aesthetic

This section comes first because it informs every visual decision. Read it before touching any token.

### Brand Personality

Cunda's visual communication should feel: **confident, warm, elegant, purposeful**.

- **Confident** — Strong hierarchy, decisive and sparing use of color, no clutter. Confidence looks like knowing what to leave out.
- **Warm** — Human photography, hand-drawn elements, a serif editorial voice. The deck should feel made by a person, not assembled by software.
- **Elegant** — Restraint is the design choice. The fewer colors in an illustration, the fewer icons on a slide, the more intentional it looks. Whitespace and fine lines communicate taste.
- **Purposeful** — Every element earns its place. If it doesn't add meaning, remove it.

### Aesthetic Direction

The visual language is rooted in **elegant restraint**. Illustrations, icons, and decorative elements live in a monochromatic, hand-drawn register — fine lines, deliberate strokes, graphite-and-ink quality. Think of a careful sketch in a professional's notebook: precise but unmistakably human.

The palette for all drawn elements is **black and white** (`#1a1a1a` on `#f5f5f4`). Color — specifically Cunda Orange — enters as punctuation, not a base coat. This restraint gives the orange far more impact when it appears.

The overall sensibility: professional without being corporate, modern without being cold, handcrafted without being casual.

---

## Design Tokens

### Colors

#### Brand Colors

| Name | Hex | Use for |
|------|-----|---------|
| **Cunda Orange** | `#FF5F1F` | Brand anchor on every slide — one accent element per slide |
| **Violet** | `#5762D5` | Secondary accents, primary chart series |
| **Green** | `#40F99B` | Growth, positive outcomes, success indicators |
| **Cyan** | `#00ADCC` | Technology, clarity, tertiary accents |
| **Red** | `#F05365` | Alerts, negative data, deliberate contrast |

Chart color sequence: **Violet → Cyan → Green → Orange → Red**

#### Neutral Colors

| Name | Hex | Use for |
|------|-----|---------|
| **Background** | `#f5f5f4` | Primary slide background — warm off-white |
| **Background Alt** | `#eeede9` | Alternate background (~3% darker, same warm family) |
| **Card** | `#fafafa` | Cards, panels, elevated surfaces |
| **Text** | `#1a1a1a` | All headlines and body text |
| **Muted** | `#595959` | Captions, secondary text, footers |
| **Border** | `#ebebeb` | Card borders, dividers |
| **White** | `#FFFFFF` | Text on colored (e.g., orange) backgrounds |

#### Background Rules

Slides always use warm light backgrounds. Two tones available — they can alternate to create visual rhythm between sections, the same way the Cunda website alternates:

- **Primary** `#f5f5f4` — warm off-white (stone family)
- **Alternate** `#eeede9` — slightly deeper warm tone, same family

**Never use `#F8FAFC`** (Tailwind `slate-50`) — it has a cool blue undertone that clashes with the warm palette.

The only exception: section divider slides, which may use a full-bleed brand color (typically Cunda Orange).

#### Using Color with Intent

- **Orange** appears on every slide — as one anchoring element (bar, headline, stat, shape). One is enough.
- **Violet / Cyan / Green** support the layout in data, charts, or card accents. Pick one or two per slide, not all at once.
- **Red** only for negative data, alerts, or a single deliberate contrast moment.
- **In illustrations and icons**: black only. Orange enters as a single accent element at most — never as a fill.

---

### Typography

#### Typefaces

| Role | Typeface | Character | PowerPoint Fallback |
|------|----------|-----------|---------------------|
| Display / Headlines | **PT Serif Bold** | Editorial authority, warmth, elegance | Georgia Bold |
| Body / UI / Captions | **Geist** (Vercel) | Neutral, geometric, high legibility | Arial |
| Emphasis | **Geist** SemiBold | Same family, weight contrast | Arial Bold |

PT Serif is the editorial voice — titles, H1, H2, H3, and large display text. Geist handles everything else: body copy, labels, captions, navigation. The pairing of a warm serif headline against a clean geometric body is central to the Cunda aesthetic.

#### Type Scale

| Level | Font | Size | Color |
|-------|------|------|-------|
| Cover Title | PT Serif Bold | 52–64pt | `#1a1a1a` (or gradient — see below) |
| Slide Title | PT Serif Bold | 30–38pt | `#1a1a1a` |
| Eyebrow / Section Label | Geist SemiBold, ALL CAPS | 11–13pt | `#FF5F1F` or `#595959` |
| Subtitle / Lead | Geist SemiBold | 18–24pt | `#1a1a1a` |
| Body | Geist Regular | 15–18pt | `#1a1a1a` |
| Caption / Footer | Geist Regular | 10–12pt | `#595959` |

#### Title Gradient (Use Once Per Deck)

A single word or short phrase in a cover or hero headline can carry the brand gradient for warmth and energy:

```
linear-gradient(90deg, #ff3131, #ff914d, #ff914d)
```

Applied as text clip (bg-clip-text / text-transparent). Use at most once per deck — on the most important headline only. It should land as a moment, not a motif.

#### Alignment & Color Rules

- **Alignment**: Left-align body text. Centered works for short isolated headings, covers, dividers, and pull quotes. Never center body paragraphs.
- **Text color**: `#1a1a1a` for all body copy. Brand colors are for one callout, label, or key stat per slide — not body text.

---

### Logo

Assets in `assets/` folder:
- `cunda-logo-full.png` — Full wordmark. Use in slide headers or footers.
- `cunda-logo-icon.png` — Infinity icon mark. Use when space is limited.

**Every slide must include the logo.** Preferred positions: top-right corner or bottom-left corner. Choose one and stay consistent within a deck.

Never distort, recolor, or apply effects to the logo.

---

## Composition Principles

These guide decisions — they don't prescribe layout.

### Lead with the Insight
The most important thing on a slide — the number, the question, the conclusion — should be the first thing the eye lands on. Don't make the audience work to find the point. If you can't identify the single most important element, rethink the slide.

### One Idea Per Slide
A slide with two ideas has none. If content naturally splits into two arguments, use two slides. Brevity forces clarity.

### Hierarchy Over Decoration
Visual weight signals importance. Big = important. Light = supporting. Orange = brand. If everything is emphasized, nothing is. Decoration that doesn't reinforce hierarchy is noise.

### Whitespace is Confidence
Empty space is not wasted space. It directs the eye, improves legibility, and signals that the deck was designed with care. A sparse, focused slide reads stronger than a dense one.

### Brand Anchor
Every content slide should include one orange element — a bar, a shape, a highlighted stat, a label. Just one. Its job is to say "this is Cunda" without shouting.

### Consistent Grid
Maintain consistent margins (approx. 40–60pt from edges). Align to an implied grid. Arbitrary placement breaks visual rhythm.

---

## Visual Language

### Icons

- **Style**: Hand-drawn or sketch-quality. Fine, slightly organic stroke weight — not pixel-perfect geometric, not rough. The line should feel considered and deliberate.
- **Color**: Always `#1a1a1a`. Reserve orange for at most one featured icon per slide — a moment of accent, not a pattern.
- **Stroke weight**: Consistent thin-to-medium across the deck. Avoid hairline extremes and heavy-fill styles equally.
- **Size**: 24–40pt for supporting icons; 48–72pt for featured or hero icons.
- **Avoid**: Filled/solid icons, 3D, skeuomorphic, clipart, or inconsistent styles within a deck. Digital-flat icon sets (Lucide, Material) only work if they can be rendered fine-line — evaluate before using.

### Illustrations & Graphics

- **Style**: Monochromatic line art. Black ink or graphite on white. Gestural but intentional — not scribbled, not over-rendered. Think architectural sketch or scientific illustration.
- **Color**: `#1a1a1a` only. One orange accent element allowed per illustration at most — as a single line or mark, never a fill.
- **Usage**: Supporting what words cannot say. A well-placed illustration creates meaning. If it doesn't add meaning, it's decoration — remove it.
- **Avoid**: Full-color illustrations, gradient fills, flat-digital vector shapes, anything that reads as generic or corporate.

### Photography

- **Style**: Editorial and understated. Prefer desaturated, near-monochromatic, or subtle-contrast treatment — so photos coexist with the hand-drawn aesthetic without competing in color.
- **Subject**: People in natural unposed moments; workspaces with texture and character; abstract material textures (paper, concrete, light); technology used by human hands. Santiago and Latin American environments welcome.
- **Treatment**: Full-bleed or contained in a card/shape. Black-and-white or low-saturation strongly preferred. Overlay text with a light or dark scrim for legibility — keep it subtle.
- **Avoid**: Vivid oversaturated stock; obvious clichés (handshakes, whiteboards, forced smiles). Color photography only when it genuinely serves the slide.

### Data Visualization

- Clean, minimal chart styles. No 3D, no shadows, no decorative chrome.
- Prefer bar, line, and donut charts. Avoid pie charts with more than 4 segments.
- Label data directly on the chart — avoid external legends where content allows.
- Highlight one key insight: make it orange or bold. Everything else recedes.
- Chart lines and axes should be as thin and unobtrusive as possible.
- Every data slide should include a one-line takeaway — the conclusion the audience should leave with.

---

## Components

### Standard Card

```
Background:    #fafafa
Border:        1px solid #ebebeb
Border-radius: 12–16px
Padding:       20–28px
```

### Accent Card

```
Background:    #fafafa
Border-left:   4px solid [brand color: #FF5F1F | #5762D5 | #40F99B | #00ADCC]
Border:        1px solid #ebebeb
Border-radius: 12px
```

**Avoid on all cards**: Dark backgrounds, gradient fills, glowing or neon effects, heavy drop shadows.

---

## Slide Roles

These describe intention and required content — not layout. Let the content and context determine the composition.

---

### Cover / Title
**Intent**: Make a strong first impression. Set the tone for the entire deck before a single word is spoken.

**Must contain**: Presentation title, subtitle or context, presenter name and role, date, location.

**For impact**: The title should do real work — not "Propuesta Cunda" but something that speaks to the specific opportunity or challenge. Use the gradient on the key word if the headline warrants it. Generous whitespace. Logo prominent.

---

### Section Divider
**Intent**: Mark a clear transition. Give the audience a moment to reset before the next chapter.

**Must contain**: Section name. Optionally a one-line description or question that frames what comes next.

**For impact**: This is the one slide that can use a full-bleed brand color (orange is the natural choice). Minimal text, maximum breathing room. The contrast with content slides creates visual rhythm.

---

### Content / Information
**Intent**: Communicate one idea clearly. Not all the information — the right information.

**Must contain**: A clear title that states the point (not just the topic), the supporting content, and an orange anchor element.

**For impact**: Lead with the conclusion in the title — "Automatización libera 30% del tiempo operativo" is stronger than "Resultados de Automatización". Use cards, columns, or a single strong visual — whatever serves the content. Leave more space than feels comfortable.

---

### Data / Metrics
**Intent**: Make a number mean something. Numbers without context don't persuade.

**Must contain**: The key stat(s), a clear label for what each number represents, and a one-line takeaway that tells the audience what to conclude.

**For impact**: Give key numbers room to breathe — large type, generous whitespace. Highlight the most important number in orange. If using a chart, the chart is the slide — don't crowd it. The takeaway line is as important as the number itself.

---

### Team / People
**Intent**: Humanize Cunda. Trust is built through people, not logos.

**Must contain**: Photo, name, role, and one sentence of relevant credential or context per person.

**For impact**: Consistent visual treatment across all team cards. Use a brand-color accent (border top or side bar) to add personality without noise. The photo should feel candid and real — editorial treatment (desaturated, natural light) preferred over corporate headshots.

---

### Quote / Testimonial
**Intent**: Let someone else say it. Third-party validation lands harder than self-description.

**Must contain**: The quote (exact words, not paraphrased), attribution (name, role, company), and ideally a logo or photo.

**For impact**: One quote per slide. Large type — the quote should dominate the slide. Generous whitespace. This slide can break from standard structure to feel more editorial and intentional. The quote earns the space it takes.

---

### Closing / Contact
**Intent**: End with energy and a clear next step. Leave the audience knowing what to do.

**Must contain**: "¡Que Cunda!" as the closing beat (PT Serif Bold Italic, large), contact name and role, email, phone, website, and one clear call to action.

**For impact**: The closing should feel like a landing, not a trailing off. "¡Que Cunda!" is distinctive — let it breathe. The call to action should be specific ("Agendemos una llamada esta semana") not generic ("Contáctanos").

---

## Narrative & Flow

Design alone doesn't make a presentation impactful — story does. A well-structured narrative makes the audience feel that the conclusion was inevitable.

### The Arc

Every Cunda deck should have a clear arc. The exact structure adapts to context, but the underlying movement is always:

**Tension → Insight → Solution → Proof → Call to Action**

1. **Open with tension** — Start with the problem, challenge, or opportunity the audience is already feeling. Don't start with the company history. Make the audience feel seen before you make them listen.

2. **Deliver the insight** — The one thing that reframes the situation. The lens through which the rest of the deck will be read. State it clearly and give it space.

3. **Present the solution** — How Cunda addresses the tension. Be specific. Avoid generic descriptions of what AI can do — ground it in their context.

4. **Prove it** — Data, case studies, client results, credentials. Evidence that the solution works. Keep it focused: one strong proof point beats five weak ones.

5. **Ask clearly** — The closing should arrive at a specific, low-friction next step. Not "get in touch" — something concrete with a timeframe.

### Slide-Level Principles

- **Every slide should move the story forward.** If a slide could be removed without breaking the narrative, remove it or find its reason to exist.
- **The title of each slide is the argument, not the topic.** "Tres razones por las que esto importa" is a topic. "El costo de no actuar crece cada mes" is an argument.
- **Don't save the best for last.** The key insight or most compelling number should appear early enough to keep attention, not as a reward at the end.
- **One slide = one takeaway.** The audience should be able to say in one sentence what each slide communicated. If they can't, the slide has too much.

---

## Confidentiality Notice

Include in the footer of all proposal slides (Geist Regular, 10–12pt, `#595959`):

```
El contenido de esta propuesta es Información Confidencial.
Prohibida su reproducción total o parcial sin autorización por escrito de Cunda SpA.
```

---

## Quick Checks

### Design
- [ ] Warm backgrounds only — `#f5f5f4` or `#eeede9` on content slides (not dark, not `#F8FAFC`)
- [ ] One orange anchor element on every slide
- [ ] Logo on every slide (consistent position across the deck)
- [ ] PT Serif for all titles and display text; Geist for body and UI
- [ ] Text color `#1a1a1a` — not white on light backgrounds
- [ ] Icons and illustrations monochromatic — consistent style throughout
- [ ] Charts: direct labels, correct color sequence, one highlighted insight
- [ ] Every slide breathes — whitespace is not empty space

### Content
- [ ] Slide titles state the argument, not just the topic
- [ ] Each slide has one clear idea
- [ ] Data slides include a one-line takeaway
- [ ] The deck has a clear arc: tension → insight → solution → proof → ask
- [ ] The closing has a specific, concrete call to action

### Compliance
- [ ] Confidentiality notice in footer on all proposal slides
