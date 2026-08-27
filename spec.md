# Spec — `implementation-v2.html`

Re-skin the AI Builders ID landing page (`implementation.html`) onto the "Editorial War Room"
design system defined in [`ai-builders-design-system.md`](./ai-builders-design-system.md).

## Goal & Scope

- **Goal:** produce `implementation-v2.html` — the *same* landing page, rebuilt on the new
  design system so it can be compared 1:1 against `implementation.html`.
- **Scope:** faithful re-skin. Sections, copy, structure, prices, names, nav anchors, and
  animations stay exactly as they are. Only the visual system changes.
- **Non-goals:** no copy rewrites, no new/removed sections (one exception: a pre-footer
  `cta-band`, see below), no dark mode, no framework/build step.

## Source Material

| File | Role |
|---|---|
| `implementation.html` | current landing page — a bundled artifact; the real page is the embedded template (old design system: kraft-tan, marker red/blue/green, Permanent Marker headlines) |
| `ai-builders-design-system.md` | the target design system spec |
| `ai-builders-design-system.html` | token/component preview of the target system — reference for exact values |

## Output Format

- Single standalone `.html` file, self-contained.
- CSS inline in one `<style>` block; JS inline in one `<script>` at end of body.
- Fonts via Google Fonts `<link>` (same as `ai-builders-design-system.html`):
  `Space Grotesk` 400–700 + `Permanent Marker`.
- No other external requests. `.ph` dashed boxes stay as image placeholders.
- Target size ~30–35 KB.

## Token Layer (`:root`)

Pull verbatim from the spec / preview file.

### Surface
| Token | Value |
|---|---|
| `--canvas` | `#fffaf0` |
| `--surface-soft` | `#faf5e8` |
| `--surface-card` | `#f5f0e0` |
| `--surface-strong` | `#ebe6d6` |

### Brand & ink
| Token | Value |
|---|---|
| `--ink` | `#0a0a0a` |
| `--ink-soft` | `#3a3a3a` |
| `--ink-faint` | `#6a6a6a` |
| `--on-dark` | `#fffaf0` |
| `--brand-pink` | `#ff4d8b` |
| `--brand-teal` | `#1a3a3a` |
| `--brand-lavender` | `#b8a4ed` |
| `--brand-peach` | `#ffb084` |
| `--brand-ochre` | `#e8b94a` |
| `--brand-mint` | `#a4d4c5` |
| `--brand-coral` | `#ff6b5a` |

### Sticky-note pastels
`--note-yellow #f2e1bf`, `--note-green #dceae4`, `--note-pink #f6dbe6`,
`--note-orange #f8dcc8`, `--note-blue #e6dff7`, `--note-purple #ddccf0`,
`--note-featured #1a3a3a` (white text).

Cycle notes/feature-cards through these without repeating a hue twice in a row.

### Hairlines
- `--hairline-ink: hsl(220 15% 18% / 0.14)` — sketch/hand-drawn elements only.
- `--hairline-flat: #e5e5e5` — clean-zone components only.

### Radius — two systems
- Wonky: `--r-sketch: 2px 8px 4px 12px`, `--r-sticky: 2px 8px 12px 4px`
- Clean: `--r-sm 8px`, `--r-md 12px`, `--r-lg 16px`, `--r-xl 24px`, `--r-pill 9999px`

### Elevation
- `--sketch-shadow: 2px 4px 10px hsl(220 15% 18% / 0.14)` — sticky notes at rest
- `--lift-shadow: 3px 6px 18px hsl(220 15% 18% / 0.20)` — hover / lifted

### Typography scale
| Token | Size | Weight | LH | Tracking | Use |
|---|---|---|---|---|---|
| display-hero | `clamp(48px, 7vw, 96px)` | 700 | 0.98 | -2.5px | hero h1 |
| display-lg | `clamp(36px, 5vw, 64px)` | 600 | 1.0 | -1.5px | major section h2 |
| display-md | `clamp(28px, 3.6vw, 40px)` | 600 | 1.1 | -0.8px | sub-heads, feature-card-flat titles, cta-band |
| title-lg | 24px | 600 | 1.25 | -0.2px | sticky-note headline, pricing plan name |
| title-md | 18px | 600 | 1.35 | 0 | card titles |
| body-lg | 19px | 400 | 1.5 | 0 | hero sub, leads |
| body-md | 16px | 400 | 1.55 | 0 | running text |
| body-sm | 14px | 400 | 1.5 | 0 | fine print, footer |
| mono-label | 12.5px | 600 | 1.4 | 1.5px, uppercase | eyebrow labels |
| hand-tag | 18px | 400 (Permanent Marker) | 1.1 | 0.01em | section tags, rotate -1.5deg |
| hand-note | 16–20px | 400 (Permanent Marker) | 1.2 | 0.01em | sticky-note handwriting, doodle callouts |
| button | 15px | 700 | 1.0 | 0 | button labels |

### Layout
- Section rhythm: `96px` vertical for major bands (`.section { padding: 96px 0 }`).
- Container: `max-width: 1280px`, `padding: 0 24px`.
- Dot-grid on body, tape pseudo-element on sticky notes, rough-underline highlighter — all preserved.

## Global Rules

1. **Headlines = Space Grotesk.** Every h1–h4, section head, and card title runs in Space
   Grotesk at the scale above. Permanent Marker never carries a headline.
2. **Permanent Marker = annotation only** — `hand-tag` section eyebrows, sticky-note
   handwriting, small SVG doodles. Never above ~24px.
3. **mono-eyebrow** — small uppercase Space Grotesk label above major section headlines,
   optionally paired with a rotated Permanent Marker `hand-tag` beside it.
4. **Two card zones:**
   - *Sketch zone* (sticky notes, sketch-border, wonky radius) → community / personality /
     storytelling sections.
   - *Clean zone* (`feature-card-flat`, `cta-band`, clean radius, no shadow) → product /
     pricing / trust sections.
5. **Teal is the "featured" signal** — one element per section max (pricing VIP tier, the
   community "what you get" panel). Full saturation, white text, never a pastel tint.
6. Section rhythm never drops below 96px on major bands.
7. No 8th brand hue. No heavy shadows on flat cards — depth there is colour vs cream.

## Colour Migration (old → new)

| Old | New |
|---|---|
| `--kraft` | `--canvas` `#fffaf0` |
| `--kraft-deep` | `--surface-strong` `#ebe6d6` |
| `--card` / `--paper` | `--surface-card` `#f5f0e0` |
| `--red` (marker) | `--brand-coral` `#ff6b5a` |
| `--blue` (marker) | `--brand-lavender` `#b8a4ed` |
| `--green` (marker) | `--brand-mint` `#a4d4c5` |
| `.btn-red / .btn-blue / .btn-green` | `.btn-coral / .btn-lavender / .btn-mint` |
| `.pill-red / -blue / -green` | `.pill-coral / -lavender / -mint` |
| `.rough-underline` red / `.hl-blue` / `.hl-yellow` | coral / lavender / ochre |
| `.section { padding: 72px 0 }` | `96px 0` |
| `h1–h4 { font-family: Permanent Marker }` | `Space Grotesk` 600–700, monumental tracking; Marker → `.hand-tag` / `.hand-note` only |
| note pastels (old hex) | new Sticky-Note Pastels table |

## Section-by-Section

Content and copy are unchanged in every row; the "Treatment" column is what changes.

| # | Section | Treatment |
|---|---|---|
| 1 | Header / nav | Sticky, `--surface-soft` at 86% + `blur(8px)`, 2px ink bottom border. Brand mark = CSS monogram tile (`--brand-teal` fill, `--on-dark` "ab", clean radius) — the old bundled logo asset is unavailable. Nav links ink; hover → coral. Buttons: "Masuk" ghost, "Gabung →" ink fill. |
| 2 | Hero | Split `1.15fr / 0.85fr` (keep the asymmetry). Left: `mono-eyebrow` "KOMUNITAS VIBE CODER" + rotated `hand-tag` "#1 di Indonesia"; h1 `display-hero`, accent word ("tanpa") in coral; sub `body-lg`; two CTAs (ink fill + ghost); fine print `body-sm` faint. Right: `hero-collage` — 3 sticky notes (note-yellow, note-blue, note-pink) with tape + `hand-note` bodies, rotated; 2 SVG doodle accents recoloured to coral + lavender. |
| 3 | About / Why | Sketch zone. `section-tag` (Permanent Marker, coral). h2 `display-lg` with coral `rough-underline` on "selesai". 3-up grid of sticky notes: note-orange (Masalah), note-green (Solusi), note-blue (Bukti), each with emoji, `title-md` head, `body-sm` body. `reveal` on each. |
| 4 | Stat | Centered. `1.400+` in **Space Grotesk** ~`clamp(56px, 9vw, 96px)` weight 700, colour coral (NOT Permanent Marker — headline rule). Supporting line `body-lg` muted, left-aligned, max 360px. |
| 5 | Builders marquee | Two opposed marquee rows. `company-chip` → `--surface-card` bg, `--hairline-flat` border, clean radius (`--r-md`), initials tile cycles brand hues. Intro block above: `section-tag` + h2 `display-md` + lead. |
| 6 | Community band | **Light flat zone** (was full-bleed ink). Background `--surface-soft`, 96px padding, `--r-xl` rounded container. Left: `section-tag` coral, h2 `display-lg`, `body-lg` lead, `.btn-mint` CTA. Right: the "Yang kamu dapat" panel as the single **teal featured card** (`--note-featured`, `--on-dark` text, `--r-xl`), 3-item list. This is the section's one featured element. |
| 7 | Pricing | Clean zone. Centered intro (`section-tag`, h2 `display-lg` with `rough-underline` "selamanya", lead). 4-tier grid (`repeat(4,1fr)` → 2 → 1). Tiers 1/2/4: `feature-card-flat` on `--surface-card` with `--hairline-flat`, `--r-xl`, no shadow. Tier 3 "Advanced VIP": teal featured card (`--note-featured`, `--on-dark`), coral `.ribbon` "PALING LARIS". Plan name `title-lg`, price Space Grotesk 700 30px, check marks mint, disabled rows faint. CTA per card. Fine print `body-sm` faint. |
| 8 | BAAPWU | Sketch zone, 2-col grid. Left: `section-tag`, h2 `display-lg` with lavender highlight on "With Us", lead, then `psp` rows each with a Permanent Marker `badge` on a note tint (orange/green/blue). `.btn-lavender` CTA. Right: sticky note-purple with tape, `title-lg` head, body, and a `.ph` placeholder recoloured to `--surface-strong` ("[ kalender cal.com ]"). |
| 9 | Sponsors marquee | Intro: `section-tag` + h2 `display-md`. `logo-pill` → `--hairline-flat` border, `--surface-card` bg, `--r-pill`, coloured dot kept. |
| 10 | FAQ | Centered intro (`section-tag`, h2 `display-lg`). `<details.qa>` → `--surface-card`, `--hairline-flat` 2px, `--r-lg`; summary `title-md`; "+" toggle in Permanent Marker coral, rotates 45° on open. |
| 11 | **CTA-band (new)** | Pre-footer. New `cta-band` component from the spec: `--surface-soft` bg, `--r-xl`, 80px padding, `display-md` headline adapted from existing copy ("Bayar sekali. Akses selamanya."), one ink CTA ("Jadi Member Eksklusif"). Optional rotated sticky note or doodle pinned at the edge. |
| 12 | Footer | **Cream / `--surface-soft`** (was ink), per the spec's "keep the footer cream/light". 5-col grid → 2-col mobile. Section headings `mono-label`. Links `body-sm` ink-soft, hover coral. Bottom bar hairline divider, `body-sm` faint. Same brand monogram tile as header. |

## Components to Build

- `.lp-header`, `.brand-tile` (CSS monogram)
- `.hero`, `.hero-collage`, `.mono-eyebrow`, `.hand-tag`, `.hand-note`
- `.sticky` + `.tape-top` + `.note-*` (7 incl. featured), `.sketch-border`
- `.section`, `.section-tag`, `.lead`
- `.btn` (+ `-ghost`, `-sm`, `-coral`, `-lavender`, `-mint`, `-clean`)
- `.pill` (+ `-coral`, `-lavender`, `-mint`)
- `.rough-underline` (+ `.hl-lavender`, `.hl-ochre`)
- `.feature-card-flat` (cycles 6 hues + cream + teal variant)
- `.cta-band`
- `.product-mockup-card` / `.ph` (dashed, `--surface-strong`)
- `.tiers` / `.tier` / `.ribbon`
- `.marquee` / `.marquee-track` / `.company-chip` / `.logo-pill`
- `.bigstat` (Space Grotesk, not Marker)
- `.faq` / `details.qa`
- `.lp-footer`
- Utilities: `.container`, `.muted`, `.faint`, `.center`, `.bg-dotgrid`, `.reveal`

## JavaScript (unchanged from source)

- `sponsors` array → `#logoTrack` (doubled for loop).
- `companies` array → `#coTrack1` / `#coTrack2` (split, doubled).
- `IntersectionObserver` adds `.in` to `.reveal` elements, threshold 0.15.
- Respect `prefers-reduced-motion` for the reveal transition (already in the base CSS).

## Responsive

Keep the source breakpoints:

| Name | Width | Behaviour |
|---|---|---|
| Mobile | < 768px | hamburger/hidden nav links; hero h1 clamps down; `hero-collage` stacks; feature grids 1-up; tiers 1-up; footer 2-col |
| Tablet | 768–1024px | feature cards 2-up; tiers 2-up |
| Desktop | 1024–1440px | full nav; 3-up feature grids; 4-up tiers |
| Wide | > 1440px | content caps at 1280px |

Body must never scroll horizontally; marquees clip inside their own `overflow: hidden`.

## Acceptance Checklist

- [ ] No Permanent Marker on any h1–h4 or the stat number.
- [ ] Every headline is Space Grotesk with negative tracking at the spec scale.
- [ ] Canvas is `#fffaf0`; no kraft-tan or pure-white page background remains.
- [ ] Only the 7 brand hues + 4 surfaces + 3 ink tones appear — no leftover `--red/--blue/--green`.
- [ ] Sketch zones (About, BAAPWU) use wonky radius; clean zones (Pricing, CTA-band, FAQ) use clean radius — never mixed.
- [ ] Exactly one teal featured element per section (community panel, pricing VIP).
- [ ] Section rhythm is 96px on major bands.
- [ ] Footer is cream/soft, not ink.
- [ ] Dot-grid, tape, and rough-underline are all present.
- [ ] All Indonesian copy, prices, sponsor/company names, and nav anchors match `implementation.html` exactly.
- [ ] Marquees animate; `.reveal` elements fade in on scroll; reduced-motion respected.
- [ ] Page body does not scroll horizontally at any width.

## Out of Scope / Notes

- Brand logo asset from the bundle is not recoverable → CSS monogram tile stands in.
- `implementation.html` is left untouched; `implementation-v2.html` is a new file.
- Commit/push happens only on explicit request.
