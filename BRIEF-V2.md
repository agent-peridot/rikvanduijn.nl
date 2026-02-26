# Website Brief v2: rikvanduijn.nl

## Goal
Rebuild the personal website. V1 was too close to govannon.nl — needs its own identity.

## Key Feedback from Rik
- Too much of a govannon.nl clone — needs to be distinctly different in layout, structure, and feel
- Projects/track record must match his ACTUAL career (see LinkedIn below)
- Do NOT mention OpenClaw
- Do NOT name Voicify — can hint at "voice synthesis tooling" or "TTS pipeline" as a side project
- Add his photo (available as `assets/rik-dancer.jpg` — him dancing, great energy shot)
- Add generated images to make site lively (available in `assets/`)
- This is NOT a "fractional CTO" pitch site — Rik is a developer who builds things

## Correct LinkedIn Experience
1. **React Native Developer** — Tired of Cancer (Untire app), Part-time, Mar 2022 – Present (~4 yrs), Utrecht
   - Cancer recovery support app, fighting Cancer Related Fatigue (CRF)
2. **React Native Developer** — Reisbalans BV, Mar 2019 – Feb 2022 (3 yrs), Amersfoort
   - Mobility/travel reimbursement platform
3. **Developer** — Inspire Innovation BV, Feb 2015 – Feb 2019 (4 yrs 1 mo), Utrecht Area
   - Web agency: websites, web applications, mobile apps
4. **Education:** Game design / design for virtual theater and games

## Design Inspiration (NOT to clone, just patterns to learn from)
- **brittanychiang.com** — clean left sidebar with sticky info, scrolling content on right, minimal but warm, hover effects on projects, great use of whitespace
- **mattfarley.ca** — personal tone ("I'm quietly confident, naturally curious"), startup projects section, mentor stats, testimonials
- **govannon.nl** — strong storytelling, timeline, service cards (but Rik's version should NOT be services-for-hire, he's a developer)

## Available Assets
All in `assets/` directory:
- `rik-dancer.jpg` — photo of Rik dancing (from his current site, credit: Kaka Lee)
- `hero-mobile.png` — abstract mobile phone with floating UI elements, amber/teal
- `section-code.png` — isometric code blocks and data streams, copper/blue
- `section-health.png` — hand holding seedling from phone screen, health tech
- `section-creative.png` — D20 dice with crystals and code, fantasy meets tech

## Rik's Personality (for tone)
- Warm, grounded, curious, precise, occasionally dry humor
- Night owl, builder, explorer
- Loves the "first 80%" — exploration and creation over polish
- Game design roots — creative thinker who became a developer
- Music lover (works at venue Doornroosje on the side)
- Values craft, friendships, doing meaningful work
- NOT corporate, NOT a consultant, NOT selling services
- A developer who happens to be really good and cares about what he builds

## What Makes Rik Different (from Claude Code insights)
- 88% goal achievement rate across 51 Claude Code sessions
- "Domain-expert driver who delegates aggressively but intervenes decisively"
- Builds across the full stack: React Native, Python, CI/CD, AWS, AI tooling
- Ships real things — from cancer recovery apps to voice synthesis pipelines to automated CI systems
- Empirical problem solver — tests, observes, course-corrects

## Design Direction
- DIFFERENT structure from govannon.nl — not sections with cards
- Consider: Brittany Chiang-style sidebar layout, or a more editorial/magazine feel, or a scrolling narrative
- Dark theme (night owl) but warmer than typical dark sites
- Use the generated images as section backgrounds or accent pieces
- The dancer photo should be prominent — it shows his energy
- Mobile-first
- Could have playful elements — he studied game design after all
- Animations/interactions welcome but tasteful
- NO frameworks — pure HTML/CSS/JS

## Sections (suggested, but be creative with structure)
1. **Intro/Hero** — photo, name, what he does, personality in one line
2. **About** — the story: game design → web dev → mobile specialist → AI-augmented builder
3. **Work** — actual career timeline with real companies and roles
4. **Side Projects** — voice synthesis tooling, CI/CD automation, AI-assisted development experiments (no names)
5. **Beyond Code** — music (Doornroosje), tabletop RPGs, house renovation — he's a whole person
6. **Contact** — LinkedIn, GitHub, email

## Tech
- Static HTML + CSS + JS
- No build step, no frameworks
- All assets in `assets/`
- Must work standalone (inline critical CSS or ensure paths work)

## Important
Delete the existing index.html and styles.css — start fresh. This is v2, not a patch.
