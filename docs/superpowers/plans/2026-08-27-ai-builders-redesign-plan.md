# AI Builders Redesign Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Create three self-contained responsive HTML redesign prototypes for AI Builders ID.

**Architecture:** Each page is a standalone HTML document with inline CSS and JS. Shared design tokens, navigation, texture, button, sticker, clay, and reveal patterns are duplicated intentionally so each file opens independently without a build step.

**Tech Stack:** HTML5, CSS3, vanilla JavaScript, local AI Builders assets, Google Fonts fallback.

**Spec:** `/home/ubuntu/documents/[2] Areas/ai-builders-design-system/ai-builders-design-system.md`

## Global Constraints

- Canvas `#FFFAF0`, soft surface `#FAF5E8`, ink `#0A0A0A`, approved accent palette only.
- Space Grotesk is the display/body family; Permanent Marker is reserved for tags and annotations.
- Sticker illustrations explain; clay is one focal animated moment per page with reduced-motion fallback.
- Use dot-grid, tape, rough underline, die-cut outline, subtle grain, and soft tinted shadows.
- No fake metrics, human/robot figures, glossy glassmorphism, or invented logos.
- All pages must work from `file://` and collapse explicitly below 760px.

### Task 1: Build standalone landing prototype

**Files:** Create `/home/ubuntu/documents/[2] Areas/ai-builders-design-system/redesign/landing.html`.

- Add responsive header, split hero, clay-style agent workshop focal, build-loop steps, sticker benefit grid, testimonial, and CTA/footer.
- Use local social preview as a texture-safe fallback and CSS clay scene when no generated media is available.
- Add mobile navigation toggle and intersection-observer reveal classes.

### Task 2: Build standalone platform prototype

**Files:** Create `/home/ubuntu/documents/[2] Areas/ai-builders-design-system/redesign/platform.html`.

- Add product shell with sidebar, workspace overview, progress panel, learning queue, and activity rail.
- Include functional nav selection, project filter buttons, and a clear empty-state message.
- Keep UI/trust layer flat; use sticker accents only for explanatory callouts.

### Task 3: Build standalone blog prototype

**Files:** Create `/home/ubuntu/documents/[2] Areas/ai-builders-design-system/redesign/blog.html`.

- Add editorial header, category rail, featured article, latest article grid, and newsletter CTA.
- Reuse local square thumbnail assets from the project so every article cover is a real sticker-style image.
- Add category filtering interaction and mobile menu toggle.

### Task 4: Verify prototypes

- Run a static HTML smoke check for required files and asset references.
- Use Playwright against `file://` URLs for desktop and mobile screenshots, nav/filter interaction, and console errors.
- Inspect git diff and report exact output paths.
