# Critical Review & Rebuild Brief v3

## Current Site Assessment

### What works ✅
- **Hero photo** — the dancer image is striking and personal, immediately differentiates from generic dev portfolios
- **Dark theme** — appropriate for the audience and personality
- **Typography** — Space Grotesk + IBM Plex Mono is a solid pairing
- **Sidebar nav on desktop** (à la Brittany Chiang) — efficient, keeps orientation
- **Scroll reveal animations** — subtle, not distracting
- **"Built at night, obviously"** footer — personality without trying too hard

### What doesn't work ❌

#### 1. Wrong value proposition
The current site says "I build things people actually use" and positions Rik as a **developer looking for a job**. The target audience is **businesses wanting a consultant/advisor**. The entire framing needs to flip from "here's my resume" to **"here's what I can do for YOUR team."**

- "I'm not looking for a new gig" in the contact section actively pushes away the target audience
- Tech chips in the hero (React Native, Python, AI Tooling) are developer shorthand, not business language
- Career timeline reads like a LinkedIn export, not a consultant's track record
- The "Side Projects" section is self-indulgent for a business audience

#### 2. Missing the consultant's key elements
Research across successful consultant sites (govannon.nl, mattfarley.ca, growth consultants) shows these convert:
- **Problem → Solution framing**: What pain does the client have? How do you fix it?
- **Social proof**: logos, testimonials, case results
- **Clear service offerings**: not "I know React Native" but "I'll get your mobile team shipping with AI"
- **Authority signals**: years of experience, industries served, team sizes mentored
- **One clear CTA**: not "say hello" but "let's talk about your team"

#### 3. Structure issues
- **Too many sections** — 5 content sections dilute the message. Consultants need: Hero → What I Do → Proof → Contact. That's it.
- **"Beyond Code"** section with hobbies has no business value. A hiring manager doesn't care about tabletop RPGs (save that for a blog or social media, not the landing page)
- **Career timeline is backwards** — businesses want to know outcomes, not employment dates

#### 4. Design issues
- **Card images with gradient overlays** are better than v1 but still feel like generic tech illustrations
- **Section numbers (01, 02, 03...)** are a Brittany Chiang pattern that's been copied too much — feels template-ish
- **Stat "88% goal achievement rate"** — means nothing to a business audience. It's a Claude Code metric.

### What best practice says

Based on research (HubSpot best-of analysis, successful freelancer/consultant sites, conversion-focused landing page patterns):

1. **Lead with the client's problem, not your identity** — "Your team is struggling with X" > "Hi, I'm Rik"
2. **Above the fold: photo + one-liner + CTA** — visitors decide in 3-7 seconds
3. **Show, don't list** — Instead of listing technologies, show outcomes: "Helped Team X ship 3x faster by introducing AI-assisted workflows"
4. **Testimonials are 10x more powerful than self-descriptions** — Even one real quote beats paragraphs of self-praise
5. **Keep it short** — One-page consultant sites that convert have 4-5 screen heights max
6. **Mobile-first is critical** — 60%+ of LinkedIn referral traffic is mobile
7. **One CTA, repeated** — The same action (book a call, send an email) should appear at least 3 times
8. **Personal warmth differentiates** — The photo, the tone, small personality touches. But in service of the pitch, not instead of it.
9. **Speed signals credibility** — No heavy frameworks, fast load, clean markup

---

## Rebuild Direction: v3

### Core repositioning
**From:** "I'm a developer, here's my history"  
**To:** "Your mobile team could be shipping faster, and I can show them how"

### Rik's actual consulting value (distilled from insights + career)
1. **AI-assisted development adoption** — He's a power user who ships with AI tools daily. He can teach teams to do the same: tool selection, governance, quality gates, workflow integration
2. **Mobile development expertise** — 7+ years React Native across health tech, mobility, agency work. Can audit, advise, and hands-on pair with teams
3. **Pragmatic process & tooling** — CI/CD automation, code quality, shipping culture. Not theoretical agile — practical "let's actually ship"
4. **Game-design systems thinking** — Unique background: approaches problems as experience design, not just code

### Tone
- Professional but not formal ("I don't do death-by-PowerPoint")
- Confident but not arrogant (contrast with Gerard's "I fix it and ask permission later")
- Warm, direct, slightly playful
- First person, short sentences, active voice

### New structure (4 sections max)

#### 1. Hero (full viewport)
- Photo (dancer image — it's unique and memorable)
- Name + one-line positioning: **"I help development teams ship better, faster, and with AI."**
- Subtitle: Mobile Development · AI Tooling · Team Enablement
- CTA button: "Let's talk" → scrolls to contact or opens mailto
- No tech chips, no buzzwords

#### 2. What I Do (the pitch)
Three clear offerings, framed as client outcomes:

**Introduce AI to Your Workflow**
Your developers are curious about AI tools but nobody's figured out how to use them productively. I've shipped production code with AI assistants for years — I'll set up the tools, establish quality gates, and get your team from experimenting to delivering.

**Level Up Your Mobile Team**
7+ years of React Native across health tech, mobility platforms, and agency work. I can audit your app architecture, pair with your developers, and help your team build apps that actually work on both platforms.

**Build Professional Structure (Pragmatically)**
CI/CD that works, code review culture that doesn't slow you down, shipping rhythms that stick. I set up the infrastructure and habits, then step back. No 200-page process documents.

#### 3. Track Record (proof, not timeline)
NOT a career timeline. Instead:
- 2-3 outcome-focused cards: "Built a cancer recovery app used by thousands" / "Automated CI/CD pipelines across multiple teams" / "11+ years building software professionally"
- If we can get even ONE testimonial quote, use it prominently
- Logos of companies worked with (Tired of Cancer, Reisbalans, Inspire Innovation) — even small logos add credibility

#### 4. Contact (clean, warm)
- Short personal note: "I'm based in Utrecht and prefer working with teams who care about their craft. No formal proposals needed — just tell me what's going on."
- Email link (prominent)
- LinkedIn link
- Maybe a subtle "I'm currently available for new engagements" indicator (green dot?)

### Design changes
- **Remove section numbers** — feels template
- **Remove sidebar nav** — for 4 sections it's overkill, use a simple fixed top bar
- **Make hero taller** — photo is the differentiator, give it space
- **Service cards: full-width, text-focused** — no need for illustrations in the pitch section, let the words do the work
- **Warmer palette** — current navy + blue accent feels cold. Try warmer: deep charcoal (#1a1a1a) with amber/copper accent, or keep navy but warm up the accent to teal-green
- **Single CTA style** — amber/copper button, used consistently throughout
- **Remove "Beyond Code"** — personality comes through in the tone and the photo, not in a section about hobbies
- **Remove "Side Projects"** — or fold the relevant ones (AI tooling, TTS pipeline) into the "What I Do" section as proof points

### Assets
- Keep `rik-dancer.jpg` (hero)
- **Remove or repurpose generated illustrations** — they add visual noise without adding business value. If kept, use ONE as a subtle background element, not per-card
- Consider generating a more professional hero variant if the dancer feels too casual for the consulting audience (but I think it works — it's memorable and human)

### Tech
- Same: static HTML + CSS + JS, no frameworks
- Inline critical CSS for performance
- Keep it under 5 screen heights on desktop

---

## Instructions for Claude Code

Read this entire file. Delete index.html and styles.css. Build from scratch based on the v3 direction above.

Key rules:
- **Frame everything as client value, not developer resume**
- **4 sections maximum**: Hero, What I Do, Track Record, Contact
- **No section numbers, no sidebar nav** — simple top bar
- **Warm dark palette** — not cold navy
- **One consistent CTA** throughout
- **Keep the dancer photo** as hero
- **GitHub link: https://github.com/isilher**
- **LinkedIn: https://www.linkedin.com/in/rikvanduijn/**
- **Email: hello@rikvanduijn.nl** (or rik@rikvanduijn.nl)
- **Do NOT mention OpenClaw, Voicify, or specific project names**
- **Do NOT include hobbies section**
- **Tone: professional but not formal, warm, direct**
- **Mobile-first, fast, clean**
