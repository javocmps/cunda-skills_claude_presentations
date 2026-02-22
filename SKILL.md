---
name: cunda-presentations
description: |
  Presentation design system for Cunda SpA. Use this skill ONLY when creating PowerPoint presentations, slide decks, or proposal documents for Cunda.

  CRITICAL: Cunda presentations use WHITE or light backgrounds. NEVER use dark backgrounds (#1A1A1A or similar). Dark colors are for TEXT only.

  Triggers: "presentation", "slides", "deck", "pptx", "propuesta", "pitch deck" combined with "Cunda"
---

# Cunda Presentation Design System

This is a **design system**, not a template library. Use these parameters to compose slides freely — the goal is visual consistency and brand coherence, not identical layouts. Each slide should look and feel like Cunda, but be tailored to its content.

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

## Color System

### Brand Colors

| Name | Hex | Personality |
|------|-----|-------------|
| **Cunda Orange** | `#FF5F1F` | Energy, action, brand identity — primary accent |
| **Violet** | `#5762D5` | Intelligence, depth — secondary accent |
| **Green** | `#40F99B` | Growth, positive outcomes |
| **Cyan** | `#00ADCC` | Technology, clarity |
| **Red** | `#F05365` | Alert, contrast, urgency |

### Neutral Colors

| Name | Hex | Usage |
|------|-----|-------|
| **Background** | `#f5f5f4` | Primary slide background — warm off-white |
| **Background Alt** | `#eeede9` | Alternate slide background (~3% darker, same warm family) |
| **Card** | `#fafafa` | Cards, panels, elevated surfaces |
| **Text** | `#1a1a1a` | All body text and headlines |
| **Muted** | `#595959` | Secondary text, captions, footers |
| **Border** | `#ebebeb` | Subtle dividers and card outlines |
| **White** | `#FFFFFF` | Text on colored backgrounds |

### Background Rule (Non-Negotiable)

Slides ALWAYS use **warm light backgrounds**. The palette has two tones that can alternate across slides or sections:

- **Primary**: `#f5f5f4` — warm off-white (stone family)
- **Alternate**: `#eeede9` — slightly deeper warm tone, same family

These two can alternate to create visual rhythm between sections, the same way sections alternate on the website.

**Never use `#F8FAFC`** (Tailwind's `slate-50`) — it carries a cool blue undertone that clashes with the warm palette.

The ONLY exception to warm backgrounds is section divider slides, which may use a full-bleed brand color (e.g., Cunda Orange).

**Never** use dark backgrounds for content slides.

### Using Color Intentionally

- **Orange**: Reserve for the brand anchor on each slide (one accent element — a bar, a shape, a highlight). It should appear on every slide.
- **Violet / Cyan / Green**: Use for supporting accents, data visualization, or secondary visual elements. Pick one or two per slide — don't use all at once.
- **Red**: Use sparingly and only for negative data, alerts, or deliberate contrast.
- **Charts**: Use this sequence → Violet → Cyan → Green → Orange → Red

---

## Typography

### Fonts

| Role | Typeface | Character | Fallback (PowerPoint) |
|------|----------|-----------|----------------------|
| Display / Headlines | **PT Serif** | Editorial authority, elegance, warmth | Georgia Bold |
| Body / UI / Captions | **Geist** (Vercel) | Neutral, geometric, high legibility | Arial Regular |
| Emphasis | **Geist** Medium/SemiBold | Same family, weight contrast | Arial Bold |

PT Serif is the editorial voice — used for H1, H2, H3 and any large display text. Geist handles everything else: body copy, labels, captions, buttons, navigation. The contrast between a warm serif headline and a clean geometric body is intentional and central to the Cunda aesthetic.

### Hierarchy

| Level | Font | Size Range | Color |
|-------|------|-----------|-------|
| Cover Title | PT Serif Bold | 52–64pt | `#1A1A1A` (or gradient on key word — see below) |
| Slide Title | PT Serif Bold | 30–38pt | `#1A1A1A` |
| Section Label / Eyebrow | Geist SemiBold, uppercase | 11–13pt | `#FF5F1F` or `#595959` |
| Subtitle / Lead | Geist SemiBold | 18–24pt | `#1A1A1A` |
| Body Text | Geist Regular | 15–18pt | `#1A1A1A` |
| Captions / Footer | Geist Regular | 10–12pt | `#595959` |

### Title Gradient (Optional Accent)

For cover slides or high-impact headings, a single word or short phrase can use the brand gradient to add warmth and energy:

```
linear-gradient(90deg, #ff3131, #ff914d, #ff914d)
applied as: bg-clip-text / text-transparent
```

Use this selectively — at most once per deck, on the most important headline. It should feel like a highlight, not a pattern.

**Alignment**: Left-align body text. Centered text works for short, isolated headings (covers, section dividers, pull quotes). Avoid centered body paragraphs.

**Color in text**: Use `#1A1A1A` for all body copy. Reserve orange or brand colors for one key callout, label, or stat per slide — not for body text.

---

## Logo

Located in `assets/` folder:
- `cunda-logo-full.png` — Full wordmark (use in headers or footers)
- `cunda-logo-icon.png` — Infinity-style icon mark (use when space is tight)

**Placement**: Every slide must include the logo. Common positions: top-right or bottom-left. Choose what works for the layout — consistency within a deck matters more than picking one absolute position.

**Rules**: Never distort, recolor, or apply effects to the logo.

---

## Layout Principles

These principles guide composition — they don't dictate structure.

### 1. Brand Anchor
Every content slide should have one orange element that anchors brand presence. This is often a top or left accent bar, but can also be an orange headline, a bold stat, a button, or a shape. One is enough.

### 2. Hierarchy Over Decoration
The visual weight of an element should reflect its importance. The most important piece of information — the insight, the number, the question — should read first. Everything else supports it.

### 3. Whitespace is a Design Element
Slides should breathe. Resist filling every corner. Generous whitespace improves legibility and communicates confidence.

### 4. Consistent Grid
Use consistent margins (recommend: 40–60px / 0.5–0.75in from edges). Align elements to an implied grid. Avoid arbitrary positioning.

### 5. One Idea Per Slide
If a slide needs two big ideas, consider splitting it. Each slide should make one clear point.

---

## Aesthetic Direction

The visual language of Cunda presentations is rooted in **elegant restraint**. Illustrations, icons, and decorative elements are conceived in a monochromatic, hand-drawn register — fine lines, deliberate strokes, graphite-and-ink quality. Think of a careful sketch in a professional's notebook: precise but unmistakably human.

The palette of illustrations and icons is primarily **black and white** (`#1A1A1A` on `#F5F5F4`). Color — specifically Cunda Orange — enters as a punctuation mark, not a base coat. This restraint gives the orange far more impact when it appears.

The overall sensibility: professional without being corporate, modern without being cold, handcrafted without being casual.

---

## Visual Language

### Icons

- **Style**: Hand-drawn or sketch-quality line icons. Fine, slightly organic stroke weight — not pixel-perfect geometric, not rough. The line should feel considered and deliberate.
- **Color**: Always `#1A1A1A` (near-black). Reserve orange (`#FF5F1F`) for at most one featured icon per slide — a moment of accent, not a pattern.
- **Weight**: Consistent thin-to-medium stroke across the deck. Avoid both hairline-thin and heavy-fill styles.
- **Size**: 24–40px for supporting icons, 48–72px for featured or hero icons.
- **Avoid**: Digital-flat UI icon sets (Lucide, Material, etc. only work if they can be styled to feel hand-drawn or very fine-line). No 3D, no skeuomorphic, no clipart, no filled/solid icons, no inconsistent styles within a deck.

### Illustrations & Graphics

- **Style**: Monochromatic line art. Black ink or graphite on white. Gestural but intentional — not scribbled, not over-rendered.
- **Technique feel**: Think architectural sketch, scientific illustration, or an elegant editorial drawing. The line does the work; fills and gradients are unnecessary.
- **Color**: Black (`#1A1A1A`) only. If a single color accent is needed, use orange — applied to one element only, not as a fill.
- **Usage**: Supporting visual elements that add meaning to the content. A well-placed illustration says what words cannot. Not decorative filler.
- **Avoid**: Full-color illustrations, gradient-heavy graphics, flat-digital vector shapes, any style that feels corporate or generic.

### Photography

- **Style**: Editorial and understated. Prefer images that are desaturated, near-monochromatic, or treated with subtle contrast — so they coexist with the hand-drawn aesthetic without competing in color.
- **Subject**: People in natural, unposed moments; workspaces with texture and character; abstract material textures (paper, concrete, light); technology used by human hands. Santiago and Latin American environments welcome.
- **Treatment**: Full-bleed or contained in a card/shape. Black-and-white or low-saturation treatment strongly preferred. If overlaid with text, use a light or dark scrim for legibility — keep it subtle.
- **Avoid**: Vivid, oversaturated stock photography; obvious clichés (handshakes, pointing at whiteboards, forced smiles). Color photography should only be used when it genuinely serves the slide.

### Data Visualization

- Clean, minimal chart styles. No 3D, no shadows, no decorative chrome.
- Prefer bar, line, and donut charts. Avoid pie charts with more than 4 segments.
- Label data directly on the chart where possible — avoid external legends when content allows.
- Color sequence: Violet → Cyan → Green → Orange → Red
- Highlight the one key insight: make it orange or bold. Everything else recedes.
- Chart lines and axes should be as thin and unobtrusive as possible.

---

## Card & Surface Patterns

Use cards and panels to group related content. Keep them light and clean.

### Standard Card
```
Background: #fafafa
Border: 1px solid #ebebeb
Border-radius: 12–16px
Padding: 20–28px
```

### Accent Card (with brand color indicator)
```
Background: #fafafa
Border-left: 4px solid [brand color]
Border: 1px solid #ebebeb
Border-radius: 12px
```

**Avoid**: Dark backgrounds on cards, gradient fills, glowing or neon effects, heavy drop shadows.

---

## Slide Roles (Not Templates)

Think of these as intentions, not rigid formats. The layout should serve the content.

**Cover / Title**: Establishes identity. Should include the presentation title, subtitle or context, presenter name, date, and location. Brand should feel strong — this is the first impression.

**Section Divider**: Marks a transition. Can use a full-bleed brand color (orange is natural). Should be visually distinct from content slides. Minimal text — just the section name and optionally a short description.

**Content / Information**: Communicates information clearly. Prioritize readability. Use cards, columns, lists, or a single strong visual — whatever the content calls for. Don't force content into a rigid grid when a different structure would be clearer.

**Data / Metrics**: Let numbers breathe. Large type for key stats. Charts should be the focus, not decoration. Include a one-line insight or takeaway.

**Team / People**: Humanizes the company. Profile cards work well — include photo, name, role, and a key credential or sentence. Keep consistent visual treatment across team members.

**Quote / Testimonial**: One strong quote, attributed clearly. Large type, generous whitespace. Can break from the standard layout to feel editorial.

**Closing / Contact**: Ends the deck with energy. Include the "¡Que Cunda!" sign-off (PT Serif Bold Italic, large), contact info, and a clear call to action.

---

## Confidentiality Notice

Include on all proposal slides in the footer (10–12pt, `#666666`):

```
El contenido de esta propuesta es Información Confidencial.
Prohibida su reproducción total o parcial sin autorización por escrito de Cunda SpA.
```

---

## Brand Voice in Design

Cunda's visual communication should feel: **confident, warm, elegant, purposeful**.

- Confident: Strong hierarchy, decisive and sparing use of color, no clutter.
- Warm: Human photography and hand-drawn elements that feel made by a person, not generated by a machine.
- Elegant: Restraint is a design choice. The fewer colors in an illustration, the fewer icons on a slide, the more intentional it looks. White space and fine lines communicate taste.
- Purposeful: Every element earns its place. If it doesn't add meaning, remove it.

The reference for this aesthetic: professional-grade craftsmanship, where the beauty is in precision and economy of means. Black and white as the default palette for all drawn elements; orange as the single exception that carries the brand's energy.

---

## Quick Checks Before Finalizing

- White or light backgrounds on content slides (not dark)
- Orange accent present on every slide (one element is enough)
- Logo on every slide
- Consistent font usage: PT Serif for titles and display text, Geist for body and UI
- Text color `#1A1A1A`, not white on light backgrounds
- Icons and illustrations are monochromatic (black) and consistent in style throughout the deck
- Color used sparingly in visuals — orange as accent, everything else B&W
- Charts labeled clearly with the correct color sequence
- Whitespace: does the slide breathe?
- Confidentiality notice in footer (proposals)
