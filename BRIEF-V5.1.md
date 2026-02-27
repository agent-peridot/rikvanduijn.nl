# Website v5.1 — Improvements

Keep the current v5 structure and visual style (navy palette, sidebar, hero dancer photo). Apply these improvements:

## Quick Wins (all required)

### Q1: Favicon
Add a simple favicon. Create an inline SVG favicon in the HTML head — the letters "rvd" in the accent color, or just a small dot in accent teal. Use `<link rel="icon" href="data:image/svg+xml,...">` approach.

### Q2: Open Graph meta tags
Add proper OG tags so LinkedIn/Telegram previews look good:
```html
<meta property="og:title" content="Rik van Duijn — Development Consultant">
<meta property="og:description" content="I help development teams ship better, faster, and with AI. Mobile development, AI integration, team enablement.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://www.rikvanduijn.nl">
<meta property="og:image" content="https://www.rikvanduijn.nl/assets/rik-dancer.jpg">
```

### Q3: Skip to content link
Add a screen-reader-friendly skip link at the top of the body.

### Q4: Compress hero image
Use `loading="lazy"` on non-hero images. Hero image is fine as-is.

## Design Improvements

### L1: Floating CTA
After scrolling past the hero, show a small floating "Let's talk →" button fixed to the bottom-right. Fade in/out based on scroll position. Same accent style as the hero CTA. Hide it when the contact section is visible.

### L3: Alternating card layouts
Instead of uniform service cards stacked the same way, alternate:
- Card 1 (AI): image-left, text-right
- Card 2 (Mobile): text-left, image-right  
- Card 3 (Testing/Compliance): image-left, text-right
- Card 4 (CI/CD): text-left, image-right

Each card should be a wide, full-content-width block with the image taking ~40% and text ~60%. On mobile, stack them (image on top, text below).

### L4: Ken Burns hero
Add a slow, subtle Ken Burns effect to the hero dancer photo. Scale from 1.0 to 1.08 over 25 seconds, then back. CSS animation, infinite, ease-in-out. Very subtle — should feel alive, not distracting.

## Image Replacements

Remove ALL AI-generated images (`hero-mobile.png`, `section-code.png`, `section-health.png`, `section-creative.png`).

Replace with these Unsplash photos (already downloaded to `assets/`):

- **Service card 1 (AI-Powered Development)**: `assets/code-dark.jpg` — dark moody code on screen
- **Service card 2 (Mobile Development)**: `assets/mobile-dev.jpg` — smartphone
- **Service card 3 (Automated Testing & Compliance)**: `assets/automation.jpg` — server/infrastructure
- **Service card 4 (CI/CD)**: `assets/team-collab.jpg` — team collaboration

- **Contact section background**: `assets/utrecht-night.jpg` — Utrecht at night. Use as a subtle background behind the contact section with a dark overlay, so the text remains readable. This grounds the "Based in Utrecht" line visually.

All Unsplash photos are free for commercial use, no attribution required.

## Content Placeholders

Add visible placeholder spots for content Rik will provide later:

1. **"How I Work" section** — between services and track record. For now, put a placeholder: three numbered steps with draft text:
   - "1. We talk" — "Tell me what's going on. No formal proposals needed."
   - "2. I embed" — "I join your team, learn the codebase, and start shipping improvements."
   - "3. I step back" — "Once the processes work and your team owns them, I move on."
   (Rik will rewrite these in his own voice)

2. **Testimonial spot** — a styled quote block between track record and contact, currently showing: *"Testimonial coming soon — ask me about references."* in a subtle italic style. Easy to swap in a real quote later.

3. **Professional headshot** — In the contact section, leave a circular placeholder (gray circle with a camera icon or just initials "RvD") where a headshot will go. Rik will provide the photo.

## What NOT to change
- Keep the hero dancer photo and current hero text
- Keep the navy/teal/amber palette
- Keep the sidebar nav on desktop
- Keep the mobile hamburger menu
- Keep the current font choices
- Keep the overall section structure (hero → what I do → track record → contact)
- Keep service card content text (just change the layout and images)

## After building
Commit all changes. Do NOT push (I'll handle that).
When finished, run: `openclaw system event --text "Done: rik-website v5.1 improvements applied" --mode now`
