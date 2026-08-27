# AI Builders Sticker Software World — Study

This study applies the shared rules in `illustrations-stickers.md` to interconnected software
systems, workflows, agent orchestration, and product explainers.

## Creative Thesis

The sticker system turns invisible software behavior into a physical editorial map. It should
feel like a builder has unpacked a system onto a cream board, separated its parts, and pinned
their relationships into view. The result is explanatory rather than decorative: every
sticker names a role through shape, placement, or connection even when it contains no text.

The signature tension is **software precision inside handmade assembly**. Windows, queues,
databases, and checkpoints remain geometrically legible, while die cuts, rotations, overlap,
grain, and ribbon paths keep the composition tactile and human.

## Visual Study

### 1. Sticker Anatomy

Every object uses the same three-part construction:

1. **Graphic core** — a flat, simplified software form with a decisive silhouette.
2. **Die-cut rim** — a clean white border, approximately 3-5% of the object's
   shortest dimension. Internal gaps do not receive a second rim.
3. **Contact shadow** — a short, soft, neutral shadow that separates layers without turning
   them into floating cards. Shadow direction stays consistent across the sheet.

Edges may be subtly irregular, but never torn, fuzzy, curled, distressed, or visibly aged.
The sticker is newly printed and confidently cut. Major foreground bodies are `#FFFFFF`; use
`#FAF5E8` only for secondary surfaces or quiet inset areas.

### 2. Shape Language

- Browser and application surfaces use broad rectangles with lightly softened corners.
- Data stores use stacked discs, trays, or compact cylinders flattened toward icon language.
- Agent stations use hubs, nodes, or workbenches; never faces, bodies, or robot heads.
- Approvals and completion use stamps, gates, checks, and closed loops.
- Inputs are open shapes; processing is clustered or circular; outputs are consolidated,
  stable shapes. This creates a visual grammar from start to finish.
- Small status pieces may be rounder and more playful than primary structural stickers.

Do not reuse one generic rounded rectangle for every role. A viewer should distinguish the
system's nouns from silhouette before inspecting their details.

### 3. Layer and Overlap

Use three explicit depth bands:

- **Board layer** — cream field and optional faint registration marks.
- **System layer** — the main software objects and connector ribbons.
- **Annotation layer** — hero title sticker or lockup, checks, cursor, spinner, marker arrow,
  or small status tabs.

Primary stickers may overlap by 8-18% of their area. Overlap should reveal dependency or
sequence, not merely fill space. Keep important silhouettes and connection endpoints visible.
Avoid stacks deeper than three stickers; beyond that, the system becomes collage rather than
explanation.

### 4. Connector Behavior

Ribbon connectors are active compositional elements, not background lines.

- Give each ribbon a clear origin and destination.
- Let it pass under one object and over another to establish system order.
- Use broad bends and one or two direction changes; avoid tangled spaghetti paths.
- Match ribbon width to hierarchy: primary flow is widest, supporting flow narrower.
- End ribbons with a tucked edge, arrow-like cut, or clean contact point.
- Use color to distinguish stages, not to imply electronics or emitted light.

At thumbnail size, the main route through the system should still be traceable.

### 5. Density and Hierarchy

Build compositions from three scales:

- **Hero scale** — title plus one dominant system object or cluster.
- **Working scale** — 3-7 supporting software objects that explain the topic.
- **Signal scale** — small statuses, nodes, tabs, and annotations used sparingly.

Simple subjects should not become sparse icon sheets. Use fewer objects but enlarge their
relationships and overlap. Complex subjects can become dense, but must preserve one dominant
route, 10-20% calm space around the title, and at least one visual pause inside the cluster.

### 6. Texture and Print Finish

Grain exists to unify the sheet, not to simulate damage. Use a fine monochrome tooth across
large fills, slightly stronger in shadows and broad color areas. Halftone may appear in one
or two secondary surfaces, but never across every object. Keep color registration clean;
occasional sub-pixel imperfection is acceptable, obvious misprint effects are not.

### 7. Camera and Framing

The canonical camera is flat-on. A tilt of up to roughly 8 degrees is acceptable when it
helps overlaps read, but verticals should remain mostly stable. The sheet is not an
architectural space: no horizon, floor-wall junction, deep perspective, or isometric room.

Recompose by format:

- **16:9 cover** — title anchors the upper-left; flow travels horizontally or diagonally.
- **4:5 social** — title and system cluster stack vertically with a compact S-curve flow.
- **1:1 tile** — central cluster wraps around a protected title block; avoid edge cropping.
- **Presentation opener** — fewer, larger stickers with stronger negative space.

### 8. Controlled Imperfection

Use imperfection at the assembly level: 1-4 degree rotations, slightly varied border widths,
offset overlap, and a hand-placed rhythm. Keep the software diagrams themselves clear and
internally aligned. If everything is crooked, nothing feels intentionally handmade.

## Composition Archetypes

Choose one archetype before generating:

- **Pipeline** — an input-to-output route for workflows, automation, deployment, and agents.
- **Constellation** — one central platform connected to several capabilities or services.
- **Workbench** — tools and active surfaces gathered around a task for tutorials or building.
- **Before / after bridge** — two states linked by a dominant transformation ribbon.
- **Layer stack** — interface, orchestration, data, and infrastructure shown as overlapping
  horizontal bands rather than a literal technical diagram.

Do not mix archetypes unless the subject genuinely requires it.

## Motion Translation

The base artwork is static. When adapted to motion, preserve the sticker metaphor:

- Stickers enter through short peel-and-place movement, not elastic UI springing.
- Connector ribbons reveal from origin to destination with a slightly uneven leading edge.
- Status markers may stamp, rotate once, or settle by 1-2 degrees.
- Use one ordered reveal through the system; avoid perpetual ambient motion everywhere.
- End on a composition identical to the static poster frame.
- Reduced-motion output uses the final poster without losing meaning.

## Failure Modes

- **Icon confetti** — many isolated symbols with no system relationship.
- **Card dashboard** — uniform UI rectangles arranged in a clean product grid.
- **Isometric diorama** — depth comes from a room or miniature architecture.
- **Scrapbook nostalgia** — torn paper, curled edges, stains, fading, or vintage distress.
- **Cable diagram** — thin glowing lines, circuit traces, plugs, or hardware language.
- **Material drift** — gloss, resin, glass, clay, chrome, or volumetric 3D lighting.
- **Hierarchy collapse** — title, nodes, and annotations all compete at the same scale.
- **Decorative complexity** — fake text, code, metrics, or controls added only to look busy.

## Production Decisions

Before using the prompt, define:

| Decision | Required input |
|---|---|
| Communication job | Cover, explainer, opener, social tile, background, or infographic |
| Core message | One sentence the viewer should understand |
| Archetype | Pipeline, constellation, workbench, bridge, or layer stack |
| Hero object | The one software form carrying the concept |
| Main route | The relationship visible at thumbnail size |
| Density | Open, balanced, or dense |
| Title | Exact supplied wording |
| Output | Exact dimensions and aspect ratio |

## Master Prompt

Create a premium AI Builders Sticker-Sheet illustration.

First understand the real communication task and the user's subject. Determine whether this
is a blog cover, service thumbnail, social image, presentation opener, infographic, brand
visual, product explanation, or background.

Exact visible title: "[EXACT TITLE]".

Visualize [TOPIC-SPECIFIC SOFTWARE METAPHOR] as an interconnected miniature software world,
rendered as if it were a sheet of clean, premium die-cut vinyl stickers layered and slightly
overlapping on a warm soft-cream surface. Build the scene from physicalized browser windows,
dashboards, workflow nodes, agent stations, task queues, databases, API gateways, approval
gates, testing checkpoints, deployment lanes, monitoring panels, and completed output
surfaces — each element rendered as its own distinct die-cut sticker shape with a bright
pure-white sticker foreground, clean white outer die-cut border, confident Ink outline where
appropriate, and a soft restrained cast shadow, as if peeled and stuck slightly askew. Use
only the components relevant to the topic.

The background must remain warm cream while foreground stickers read as noticeably brighter
pure-white vinyl. Do not make major sticker bodies cream, ivory, beige, yellowish white, pale
gray, or the same color as the canvas. The white sticker layer must visibly pop against the
warm cream surface.

Use adaptive density. A simple topic may use fewer zones, but must still contain multiple
connected sticker-software elements, visible system relationships, layered overlap depth, and
a purposeful miniature composition. A complex topic may fill the frame edge-to-edge like a
densely packed sticker sheet, while staying legible — never let it collapse into a few
isolated icons floating in empty space.

Do not include any human figures, characters, hands, or body parts of any kind, cartoon or
otherwise. Keep the scene entirely about the software elements themselves. To suggest the
system is active and in motion, use small non-human activity markers instead: a cursor/pointer
sticker resting on a panel, a small "in progress" spinner sticker on a checkpoint, a checkmark
sticker on an approval gate, a subtle motion-trail along a connector. These markers are
optional accents, not a focal subject — if the scene reads better calm and static, omit them
entirely.

Camera: flat-on or very slight top-down tilt, like looking directly at a sticker sheet or a
laptop lid — not a deep 3/4 isometric room. Depth comes from sticker overlap, layered
shadow, and z-order, not from a receding architectural interior.

Rendering finish: flat vector-illustration base with a fine, subtle film-grain / halftone
texture as a light overall tooth — present across surfaces but restrained, closer to the
grain in a printed sticker or riso print than a rough paper texture. Edges stay crisp and
confidently outlined (typical clean sticker die-cut border), fills stay flat and smooth at a
glance, with the grain only visible on close inspection. No gradients used as a substitute
for the grain. The scene must read as a crisp, new, flat sticker sheet — never as worn,
creased, crumpled, faded, or aged material.

Palette — Whiteboard system: Canvas Cream #FFFAF0 is the primary background and negative
space. Sticker White #FFFFFF is the primary foreground body for die-cut cards, browser
windows, application panels, and major software surfaces. Surface Soft #FAF5E8 is restricted
to secondary board surfaces, quiet inset areas, and disabled states; never use it as a major
foreground body. Ink #0A0A0A is for titles, keylines, icons, and structural linework; Ink
Faint #6A6A6A is for secondary details and subtle grain shadow. Use controlled but clearly
visible accent hues on focal controls, workflow states, headers, nodes, status indicators,
and selected interface elements, drawn only from: Brand Pink
#FF4D8B, Brand Teal #1A3A3A, Brand Lavender #B8A4ED, Brand Peach #FFB084, Brand Ochre #E8B94A,
Brand Mint #A4D4C5, Brand Coral #FF6B5A. Do not introduce hues outside this set.

Keep approximately 60-70% of structural sticker surfaces pure white, 20-30% in controlled
accent fills, and the remainder in Ink details. For colored objects use: accent fill, optional
Ink linework, white die-cut rim, then contact shadow. For white software surfaces use:
pure-white fill, thin Ink keyline, optional narrow white safety edge, then contact shadow.

Use colored ribbon-sticker connector strips (like a strip of washi tape or a colored sticker
banner) to communicate data, orchestration, task movement, approvals, and system connections
between elements. These connectors must read as flat sticker strips with the same light grain,
never as electrical cables, glowing digital light-trails, or hardware wiring.

Materials read as exactly one thing: matte vinyl sticker with a light grain texture and a
die-cut outline. No glass, no resin, no glossy acrylic, no painted metal, no chrome, no
3D-rendered depth, no soft-shadow-heavy claymorphism.

Place the exact uppercase title flat in clean upper-left negative space, styled as one large
hero sticker or a flat title lockup with its own subtle outline. The title sticker uses
Sticker White #FFFFFF and must clearly contrast with Canvas Cream #FFFAF0. It should occupy
approximately 25-35% of the composition and remain readable at thumbnail size. Use Ink
#0A0A0A by default, set in a tight, confident geometric sans (not handwriting). Add no other
visible text unless explicitly requested. A small handwritten-marker annotation (a short
circled word or arrow, in Brand Coral) may appear near the title as a secondary sticker
accent, echoing the site's hand-marker system — never as the main title itself.

Avoid glossy resin/acrylic rendering, painted metal, glass UI layers, deep 3/4 isometric room
interiors, paper-craft/diorama cut-paper styling, worn or crumpled or creased or faded
texture, botanical decoration, watercolor, cool blush-gray or neon rainbow palettes, dominant
black backgrounds, cyberpunk, uncontrolled neon, generic corporate offices, any human or
humanoid figures, hands, robots, robot heads, circuit boards, electrical cables, plugs,
switches, relays, server racks, industrial machinery, real logos, watermarks, garbled text,
unrelated labels, decorative code, fake data, or foreground stickers that blend into the
cream canvas.

Output: [DIMENSIONS AND ASPECT RATIO]. Recompose the sticker world specifically for that
canvas; do not make a blind crop of another format.

## Text Rules

- Base all visible text on user input.
- Preserve a complete supplied title exactly.
- For short covers, use one dominant title sticker and no other visible words.
- Keep the title flat rather than placing it on an angled or curled sticker.
- The title must occupy approximately 25-35% of the composition.
- Do not invent slogans, fake metrics, decorative code, or random English.

## Composition Rules

- Canonical camera: flat-on or slight top-down sticker-sheet view — not a deep isometric room.
- Primary direction: AI Builders Sticker-Sheet Software World.
- Density policy: adaptive density with a minimum of multiple connected, overlapping sticker elements.
- Depth comes from sticker overlap and layered shadow, not architectural recession.
- Foreground sticker surfaces use Sticker White #FFFFFF; the background remains Canvas Cream
  #FFFAF0.
- Grain/film-texture stays fine and subtle — a light tooth visible only on close inspection, never heavy, rough, or worn.
- Keep a clear title zone and an interconnected sticker cluster as the visual core.
- Use ribbon-sticker connectors for system movement; never electrical wiring or light-trails.
- Use white foreground stickers as the dominant structural layer, with controlled accent
  colors providing hierarchy.
- No human figures; suggest activity only through optional non-human markers (cursor, spinner, checkmark, motion-trail).

## Review Checklist

- [ ] The scene reads as a layered sheet of die-cut stickers, not a 3D diorama or isometric room.
- [ ] Foreground sticker bodies are bright pure white #FFFFFF.
- [ ] Background remains warm cream #FFFAF0 and is visibly darker/warmer than the stickers.
- [ ] Surface Soft #FAF5E8 appears only in secondary or inset areas.
- [ ] Film-grain is fine and subtle — visible only on close inspection; the sheet reads crisp and new, not worn, creased, or faded.
- [ ] Adaptive density matches the topic without becoming sparse or empty.
- [ ] The exact title occupies roughly 25-35% and reads at thumbnail size.
- [ ] Only the 7 design.md accent hues appear, on the cream/soft base.
- [ ] Ribbon-sticker connectors read as tape/sticker strips, not cables or glowing lines.
- [ ] No glossy resin, glass, metal, or paper-craft diorama styling has crept back in.
- [ ] No human or humanoid figures, hands, robots, electronics, logos, watermarks, or extra text.

## User Input

`{phrase, topic, or short copy}`
