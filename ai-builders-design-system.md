# AI Builders ID — Design System
### "Editorial War Room" — Whiteboard visual language × warm-cream palette × editorial typography

## Overview

AI Builders ID keeps its **Digital Whiteboard / War Room** soul — kraft-board canvas, sticky notes with tape, hand-sketched wonky borders, dot-grid texture, rough-marker highlights — but is re-lit with a **warm cream + saturated 6-color palette** and re-typeset with a **monumental, tight-tracking editorial hierarchy**.

The synthesis works because of one lucky coincidence: the new 6-color feature-card palette (pink, teal, lavender, peach, ochre + cream) maps almost 1:1 onto the site's existing 6-color sticky-note system. Recoloring the notes with these hues is not a stretch — it's the same pattern both systems already share.

The bigger move is typographic. The target editorial voice is a giant, tight, negatively-tracked display face — the opposite personality of a marker scrawl. Rather than replace the handwritten identity outright, **Permanent Marker is demoted from "headline font" to "annotation font"** (section tags, sticky-note titles, badges, doodled circles/arrows), and headlines move to **Space Grotesk run at monumental scale and tracking** — which works cleanly because Space Grotesk is a well-supported display face built for exactly this treatment. The result: a monumental, editorial headline with a handwritten annotation scribbled next to it — command-center clarity with war-room texture.

**Key Characteristics:**
- Canvas shifts from tan-kraft to a warm cream (`#fffaf0`) — still reads as "board," now brighter and more premium.
- 6-color saturated palette (pink / teal / lavender / peach / ochre / mint+coral as secondary accents) drives sticky notes, pills, highlighter marks, and CTA variants — replacing the old ad-hoc red/blue/green marker set.
- Two card languages coexist by zone: **wonky sketch cards** (sticky notes, testimonials, doodled callouts) for community/personality sections, and **clean flat cards** (feature cards, CTA bands, pricing) for product/trust sections.
- Headlines run monumental and tight in Space Grotesk; Permanent Marker is reserved for annotations, tags, and sticky-note handwriting only.
- Section rhythm opens up from 72px to 96px — more premium breathing room without losing density where it earns its keep (feature grids, research-style lists).
- Cream/light footer — already the site's default, no change needed.
- Dot-grid + sketch-border + tape + rough-underline highlighter — fully preserved as the tactile, hand-crafted signature.

## Colors

### Brand & Accent
- **Ink / Primary** (`{colors.primary}` — `#0a0a0a`): CTA buttons, sketch-border strokes, h1–h4 ink, primary button fill.
- **Brand Pink** (`{colors.brand-pink}` — `#ff4d8b`): Sticky note, pill, highlighter, feature-card variant.
- **Brand Teal** (`{colors.brand-teal}` — `#1a3a3a`): Reserved for the "featured / pinned" signal — dark sticky note, featured pricing card. Not used as a pastel tint (too dark) — used at full saturation, sparingly, the way a featured pricing tier leans on a single dark accent.
- **Brand Lavender** (`{colors.brand-lavender}` — `#b8a4ed`): Replaces the old "marker blue" role — pills, links-on-hover, sticky note, CTA variant.
- **Brand Peach** (`{colors.brand-peach}` — `#ffb084`): Sticky note, feature-card variant.
- **Brand Ochre** (`{colors.brand-ochre}` — `#e8b94a`): Sticky note, feature-card variant.
- **Brand Mint** (`{colors.brand-mint}` — `#a4d4c5`): Replaces the old "marker green" role.
- **Brand Coral** (`{colors.brand-coral}` — `#ff6b5a`): Replaces the old "marker red" role — danger/urgency CTAs, hero accent word.

### Surface
- **Canvas** (`{colors.canvas}` — `#fffaf0`): Default page/board background.
- **Canvas Soft** (`{colors.surface-soft}` — `#faf5e8`): Footer, CTA-band background, sticky header (with blur).
- **Card / Paper** (`{colors.surface-card}` — `#f5f0e0`): Base "paper" fill for sticky notes and clean cards before hue tint is applied.
- **Surface Strong** (`{colors.surface-strong}` — `#ebe6d6`): Dashed image-placeholder background, deeper divider bands, emphasized rows.

### Sticky-Note Pastels (brand hues, tinted to note-lightness ~86–90% L)
Each note color is the *same hue* as a brand color, lightened to sticky-note range. This keeps the note system and the feature-card system visually related, not arbitrary.

| Note token | Derived from | Hex (approx) |
|---|---|---|
| `{colors.note-yellow}` | ochre tint | `#f2e1bf` |
| `{colors.note-green}` | mint tint | `#dceae4` |
| `{colors.note-pink}` | pink tint | `#f6dbe6` |
| `{colors.note-orange}` | peach tint | `#f8dcc8` |
| `{colors.note-blue}` | lavender tint (light) | `#e6dff7` |
| `{colors.note-purple}` | lavender tint (deep) | `#ddccf0` |
| `{colors.note-featured}` | brand-teal, full saturation | `#1a3a3a` (white text) |

Cycle notes/feature-cards through this list without repeating the same color twice in a row (the same no-repeat rule the feature-card grid uses).

### Text
- **Ink** (`{colors.ink}` — `#0a0a0a`): Headlines, primary text.
- **Ink Soft** (`{colors.ink-soft}` — `#3a3a3a`): Default running body text.
- **Ink Faint** (`{colors.ink-faint}` — `#6a6a6a`): Sub-headings, captions, footer body, metadata.
- **On Dark** (`{colors.on-dark}` — `#fffaf0`): Text on the featured-teal note/card and on primary ink buttons.

### Hairlines & Borders
- **Hairline Ink** (`hsl(220 15% 18% / 0.14)`): The *existing* translucent-ink hairline — keep for all hand-drawn/sketch-border elements. This is what makes sketch borders read as pen strokes, not flat UI lines.
- **Hairline Flat** (`{colors.hairline}` — `#e5e5e5`): New — reserved for the clean flat-zone components only (feature-card-flat, forms, product-mockup-card).

### Semantic
- **Success** — `#22c55e`
- **Warning** — `#f59e0b`
- **Error** — `#ef4444`

## Typography

### Font Family
- **Display**: `'Space Grotesk'`, weight 600–700, run at monumental scale/tracking. Fallback: `-apple-system, BlinkMacSystemFont, sans-serif`.
- **Body**: `'Space Grotesk'`, weight 400.
- **Annotation / Hand**: `'Permanent Marker', cursive` — annotation-only role (see Principles).
- **Mono / Eyebrow Label**: `'Space Grotesk', monospace` fallback, uppercase, letter-spaced — an editorial mono-label pattern, reused for eyebrow tags above section headlines.

### Hierarchy

| Token | Size | Weight | Line Height | Letter Spacing | Use |
|---|---|---|---|---|---|
| `{typography.display-hero}` | `clamp(48px, 7vw, 96px)` | 700 | 0.98 | -2.5px | Homepage hero h1 |
| `{typography.display-lg}` | `clamp(36px, 5vw, 64px)` | 600 | 1.0 | -1.5px | Major section h2 |
| `{typography.display-md}` | `clamp(28px, 3.6vw, 40px)` | 600 | 1.1 | -0.8px | Sub-section heads, feature-card-flat titles |
| `{typography.title-lg}` | 24px | 600 | 1.25 | -0.2px | Sticky note headline, pricing plan name |
| `{typography.title-md}` | 18px | 600 | 1.35 | 0 | Card titles |
| `{typography.body-lg}` | 19px | 400 | 1.5 | 0 | Hero sub-line, lead paragraphs |
| `{typography.body-md}` | 16px | 400 | 1.55 | 0 | Default running text |
| `{typography.body-sm}` | 14px | 400 | 1.5 | 0 | Footer body, fine print |
| `{typography.mono-label}` | 12.5px | 600 | 1.4 | 1.5px, uppercase | Eyebrow labels above section headlines |
| `{typography.hand-tag}` | 18px | 400 (Permanent Marker) | 1.1 | 0.01em | Section tags, rotated -1.5deg |
| `{typography.hand-note}` | 16–20px | 400 (Permanent Marker) | 1.2 | 0.01em | Sticky-note handwriting, doodled callouts |
| `{typography.button}` | 15px | 700 | 1.0 | 0 | Button labels |

### Principles
- **Space Grotesk carries the hierarchy.** All headlines (h1–h4, section heads, card titles) run in Space Grotesk at large size, tight line-height, and negative tracking — this is where the monumental editorial feel lives.
- **Permanent Marker is annotation-only.** It never carries a primary headline again. Its job: section eyebrow tags, sticky-note titles/handwriting, small doodled call-outs (circles, arrows, underlines drawn as SVG). Treat it the way a person would actually scribble on a printed page — small, off-angle, secondary to the printed type.
- **Mono-label eyebrows are new.** Pair one above major section headlines: a small uppercase Space Grotesk tag, optionally with a Permanent Marker tag rotated next to it — "official label" + "handwritten annotation" layered together.
- Never let hand-marker type exceed ~24px — past that it competes with the display hierarchy instead of supporting it.

## Layout

### Spacing System
- **Base unit:** 4px (unchanged).
- **Section padding:** bumped from 72px → `{spacing.section}` 96px for major editorial bands. Feature grids, research-style lists, and dense product sections may keep tighter internal spacing — the *between-section* rhythm is what opens up, not every internal grid.
- **Card padding:** 24–32px, unchanged.

### Grid & Container
- **Max content width:** 1200–1280px centered (bumped slightly from 1180px for a more premium rhythm).
- **Hero:** keep the existing 1.15fr/0.85fr split (headline left, sticky-note collage right) — this asymmetry is a signature, don't square it off.
- **Feature grids:** 3-up desktop / 1-up mobile, alternating sticky-note and feature-card-flat components.

### Whitespace Philosophy
Whitespace now does double duty: it's still the "board with room to pin things" feeling, but with the more generous section gaps it also reads as trustworthy/premium rather than purely playful — closer to "a well-organized war room" than "a cluttered one."

## Elevation & Depth

| Level | Treatment | Use |
|---|---|---|
| Flat | No shadow | `feature-card-flat`, `cta-band`, nav, hero copy |
| Sketch shadow | `2px 4px 10px hsl(220 15% 18% / 0.14)` (softened from 0.16) | Sticky notes at rest |
| Lift shadow | `3px 6px 18px hsl(220 15% 18% / 0.20)` | Sticky notes on hover, lifted cards |
| Tape | Existing `.tape-top` pseudo-element | Sticky notes only |

The shadow opacity is slightly softened to sit comfortably on the brighter cream — the old values were tuned for the darker kraft-tan and read a touch heavy on `#fffaf0`.

## Shapes

### Border Radius — two systems by zone

**Wonky (hand-drawn zone)** — unchanged, keep for all sticky notes, testimonial cards, doodled callouts:
- `{rounded.sketch}` — `2px 8px 4px 12px`
- `{rounded.sticky}` — `2px 8px 12px 4px`

**Clean (product/trust zone)** — new, for feature-card-flat / cta-band / product-mockup-card / pricing:
- `{rounded.sm}` — 8px
- `{rounded.md}` — 12px (buttons, inputs)
- `{rounded.lg}` — 16px (content cards)
- `{rounded.xl}` — 24px (feature-card-flat, cta-band)
- `{rounded.pill}` — 9999px (pills, tags)

Buttons stay on the wonky sketch radius by default (personality-forward CTA) — use the clean 12px radius only inside clean-zone components (e.g. a "Book a demo" button embedded in a pricing card).

## Components

### Kept as-is
- **`lp-header`** — sticky nav, blurred cream background. Recolor background to `{colors.surface-soft}` at 86% opacity.
- **`sketch-border`** — hand-drawn card border. Unchanged, still uses hairline-ink + ink stroke.
- **`ph` (dashed placeholder)** — unchanged, recolor background to `{colors.surface-strong}`.
- **`hero-collage`** — sticky-note collage in hero. Recolor notes per the new palette.

### Recolored
- **`sticky` / `.note-*`** — 6 notes + 1 featured-teal note, per the Sticky-Note Pastels table above.
- **`btn-red` → `btn-coral`**, **`btn-blue` → `btn-lavender`**, **`btn-green` → `btn-mint`** — same shape/behavior, new hues.
- **`pill-red/blue/green` → `pill-coral/lavender/mint`** — same shape, new hues.
- **`rough-underline` / `.hl-*`** — recolor to coral / lavender / ochre (from red / blue / yellow).
- **`section-tag`** — stays Permanent Marker, recolor to `{colors.brand-coral}` (from plain red).

### New
- **`feature-card-flat`** — saturated flat card, `{rounded.xl}` (24px), no shadow, cycles through the 6 brand hues. Holds an h3 in `{typography.title-md}`, a short body line, and a small product-UI fragment or icon. Text flips to `{colors.on-dark}` on the teal variant, stays `{colors.ink}` on the rest.
- **`cta-band`** — closing pre-footer band, `{colors.surface-soft}` background, `{typography.display-md}` headline, primary CTA. Rounded `{rounded.xl}`, padding 80px. Optional sticky-note or doodle pinned at the edge for continuity with the rest of the page.
- **`mono-eyebrow`** — small uppercase Space Grotesk label (`{typography.mono-label}`) placed above section headlines, optionally paired with a rotated Permanent Marker tag beside it.
- **`product-mockup-card`** — clean card (hairline-flat border, `{rounded.lg}`) for showing actual product UI/screenshots, distinct from the wonky sticky-note treatment.

## Do's and Don'ts

### Do
- Cycle the 6 brand hues across sticky notes and feature-card-flat components; don't repeat a hue twice in a row.
- Keep Permanent Marker under ~24px and off primary headlines — annotation only.
- Use `feature-card-flat` / `cta-band` for product, pricing, and trust-building sections; use sticky notes / sketch-border for community, personality, and storytelling sections.
- Keep the dot-grid, tape, and rough-underline highlighter — they're the tactile signature and nothing here replaces them.
- Use the teal note/card sparingly, as the "featured/pinned" signal — not as a general-purpose 7th color.
- Keep the footer cream/light — it's already the site default.

### Don't
- Don't put Permanent Marker on an h1 again — that's the one hierarchy rule this system exists to fix.
- Don't apply the wonky sketch radius to clean-zone components (pricing, product mockups) — it'll read as a mistake, not a style choice.
- Don't drop the section rhythm back to 72px on major bands — 96px is now the default.
- Don't invent an 8th brand hue outside the defined set.
- Don't add heavy drop shadows to the new flat cards — depth there comes from color contrast against cream, not shadow.

## Responsive Behavior

Unchanged breakpoints, existing collapsing strategy stays:

| Name | Width | Key Changes |
|---|---|---|
| Mobile | < 768px | Hamburger nav; hero h1 clamps down; hero-collage stacks below; feature grids 1-up |
| Tablet | 768–1024px | Feature cards 2-up |
| Desktop | 1024–1440px | Full nav; 3-up feature/sticky grids |
| Wide | > 1440px | Max content 1280px, more breathing room |

## Iteration Guide

1. Start any new section by deciding its zone: **playful/community** (sticky notes, sketch-border, wonky radius) or **product/trust** (feature-card-flat, cta-band, clean radius). Most pages will alternate both.
2. Set the headline first in Space Grotesk at the right hierarchy level — never reach for Permanent Marker for the headline itself.
3. If the section wants a handwritten touch, add a `mono-eyebrow` + rotated Permanent Marker tag *next to* the headline, not instead of it.
4. Pick sticky-note/feature-card colors by cycling the palette table — never eyeball a hex.
5. Reserve teal (`{colors.brand-teal}`) for one "featured" element per section, max.
6. Keep dot-grid + tape + rough-underline on every page — they're non-negotiable brand signature, same status as the cream canvas or the tight display tracking.

## Migration Notes (old token → new token)

| Old | New |
|---|---|
| `--kraft` (`hsl(39 30% 93%)`) | `{colors.canvas}` `#fffaf0` |
| `--kraft-deep` | `{colors.surface-strong}` `#ebe6d6` |
| `--card` | `{colors.surface-card}` `#f5f0e0` |
| `--red` | `{colors.brand-coral}` `#ff6b5a` |
| `--blue` | `{colors.brand-lavender}` `#b8a4ed` |
| `--green` | `{colors.brand-mint}` `#a4d4c5` |
| `--note-yellow/green/pink/blue/orange/purple` | see Sticky-Note Pastels table (same names, new hex, +1 `note-featured`) |
| `h1, h2, h3, h4 { font-family: 'Permanent Marker' }` | `font-family: 'Space Grotesk'`, weight 600–700, monumental-scale tracking. Permanent Marker moves to `.hand-tag` / `.hand-note` utility classes only. |
| `.section { padding: 72px 0 }` | `.section { padding: 96px 0 }` |

## Known Gaps

- Exact pastel hex values in the Sticky-Note table are computed approximations (same-hue tint at note-lightness) — fine-tune by eye once implemented against the actual `#fffaf0` canvas.
- This doc doesn't re-derive every existing micro-component (`.font-hand`, `.container`, scrollbar styling, `.reveal` animation) — those are unaffected and carry over unchanged.
- The mono-label / eyebrow pairing pattern is new and untested on this site — worth a quick visual QA pass on one section before rolling out everywhere.
- Illustration style (any custom SVG/doodle assets beyond CSS-driven sticky notes and dot-grid) isn't covered — heavily rendered 3D illustrations are explicitly **not** adopted here; this system stays flat/CSS-drawn, consistent with the existing site.
