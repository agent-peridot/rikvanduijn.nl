# Website Brief v4: Bento Grid — Unique Layout

## The Problem with v3
Same consulting template structure as govannon.nl — Hero → Services → Proof → Contact in linear scroll. Different content, same skeleton. Rik wants something that looks and feels genuinely unique.

## The Solution: Bento Grid Layout
A mosaic/grid-based layout where the entire page is a composition of tiles at varying sizes. Think Apple keynote feature grids, dashboard aesthetics, a mood board that doubles as a professional pitch.

**Why this fits Rik:**
- Game design background → spatial composition, not linear narrative
- Visually distinctive — almost no consulting sites use this approach
- Modern, current (2025-2026 trend but not yet overdone for consultants)
- Natural mobile responsiveness — tiles just stack
- Allows mixing photo, text, stats, and CTAs without rigid sections

## Layout: The Grid

### Desktop (3-4 column grid)
Imagine a grid with gaps. Each tile is a card with rounded corners, subtle glass/surface feel.

```
┌─────────────────┬──────────┬──────────┐
│                  │          │          │
│   HERO TILE      │  PHOTO   │  STAT    │
│   Name + tagline │  Dancer  │  11+ yrs │
│   + CTA          │  image   │          │
│                  │          │          │
├──────────┬───────┴──────────┤──────────┤
│          │                  │          │
│ SERVICE  │   SERVICE 2      │ SERVICE  │
│ AI       │   Mobile Teams   │ Process  │
│ Adoption │                  │          │
│          │                  │          │
├──────────┴──────────┬───────┴──────────┤
│                     │                  │
│  PROOF / OUTCOMES   │   COMPANIES      │
│  "Built a health    │   Logos or names  │
│   app used by       │   Tired of Cancer │
│   thousands"        │   Reisbalans      │
│                     │   Inspire         │
├──────────┬──────────┴──────────────────┤
│          │                             │
│ QUOTE    │       CONTACT               │
│ (if any) │  "Let's talk" + email       │
│          │  LinkedIn / GitHub          │
│          │                             │
└──────────┴─────────────────────────────┘
```

### Mobile: tiles stack in a sensible order (hero → photo → services → proof → contact)

## Design System

### Palette (warm dark)
- Background: `#111111` (near black)
- Tile surface: `#1a1a1a` with subtle border `#2a2a2a`
- Accent: copper/amber `#d4915c` — warm, inviting, stands out
- Secondary accent: soft teal `#5bb8a9` — for variety without clashing
- Text primary: `#f0ece6` (warm white, not blue-white)
- Text secondary: `#8a8478` (warm gray)
- CTA button: amber `#d4915c` background, dark text

### Typography
- Headings: Space Grotesk (already chosen, works well)
- Body: Inter or Space Grotesk
- Mono accents: IBM Plex Mono for labels/tags

### Tile styles
- Rounded corners (16px)
- Subtle border (1px solid #2a2a2a)
- Some tiles can have gradient backgrounds (subtle, dark-to-slightly-less-dark)
- Photo tile: no border, image fills entirely
- Hover: slight lift (translateY -4px) + border brightens
- Gaps between tiles: 12-16px

### Interactions
- Scroll reveal: tiles fade in with slight scale (0.95 → 1.0)
- Stagger: tiles reveal in sequence, not all at once
- CTA tiles: subtle pulse or glow on hover
- Keep it classy — no particle effects or 3D transforms

## Content Per Tile

### Hero tile (large, spans 2 columns)
```
Rik van Duijn

I help development teams
ship better, faster, and with AI.

[Let's talk →]
```

### Photo tile (tall, 1 column)
The dancer photo. Full bleed, rounded corners. No overlay text — let the image breathe.

### Stat tile (small, 1 column)
```
11+
years building
software
```

### Service tile 1 — AI Adoption
```
AI in Your Workflow

Your team is curious about AI tools but nobody
knows how to use them productively yet. I do —
daily. I'll set up the tools, quality gates, and
get your team from experimenting to delivering.
```

### Service tile 2 — Mobile Teams (larger tile)
```
Mobile Development

7+ years of React Native. Health tech, mobility
platforms, agency projects. I audit architectures,
pair with developers, and help teams build apps
that actually work.
```

### Service tile 3 — Process
```
Structure That Ships

CI/CD, code review culture, shipping rhythms.
I build the infrastructure and habits, then
step back. No 200-page process documents.
```

### Proof tile (spans 2 columns)
```
Track Record

Cancer recovery app used by thousands of patients.
Automated CI/CD pipelines across multiple teams.
AI-assisted development workflows shipping daily.
Full-stack across React Native, Python, AWS, and more.
```

### Companies tile
```
Worked with

Tired of Cancer · Reisbalans · Inspire Innovation
```
(Just names in a clean row, possibly with subtle styling)

### Contact tile (large)
```
Let's talk

Based in Utrecht. I work with teams who care
about their craft. No formal proposals needed —
just tell me what's going on.

[hello@rikvanduijn.nl →]

🟢 Available for new engagements

LinkedIn · GitHub
```

### Optional: Quote tile (if we have a testimonial)
If no real testimonial, skip this tile entirely. Do NOT make up a quote.

## Key Rules for Builder
1. **CSS Grid is king** — use `grid-template-areas` for the layout, with named areas
2. **Mobile: single column stack** — tiles go full width
3. **Tablet (768px+): 2 columns**
4. **Desktop (1024px+): 3-4 columns**
5. **No sidebar, no traditional nav** — the page IS the grid, it's all visible
6. **If it scrolls, it's only because the grid is tall** — not because there are "sections"
7. **Keep total height reasonable** — 3-4 scroll heights max on desktop
8. **Inline critical CSS** for fast load
9. **The dancer photo tile should be one of the first things you see**
10. **CTA appears in hero tile AND contact tile minimum**
11. **Assets available:** `assets/rik-dancer.jpg`, generated images in `assets/` (use sparingly as tile backgrounds if they work, don't force them)

## What NOT to do
- No linear section-by-section layout
- No sidebar navigation
- No section numbers
- No career timeline
- No hobbies section
- No tech skill chips/badges
- No generated illustrations as card images (they looked generic)
- No "88% goal achievement" or Claude Code stats
- Don't clone any existing site's structure

## Inspiration
- Apple feature grids (product pages)
- Bento grid dashboards
- Notion-style card layouts
- The feeling of opening a well-organized game inventory screen
