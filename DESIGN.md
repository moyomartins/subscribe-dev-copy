<!-- SEED: re-run /impeccable document once there's code to capture the actual tokens and components. -->

---
name: subscribe.dev
description: Drenched-ultramarine marketing site for premium AI billing infrastructure
---

# Design System: subscribe.dev

## 1. Overview

**Creative North Star: "International Billing Blue"**

One color owns this brand the way Yves Klein owned his blue. The page surface IS ultramarine: not an accent, not a hero band that gives way to safe white, but the ground the whole site stands on. Against it, only white type and white objects. The effect is a campaign poster for infrastructure: fast, bold, opinionated, impossible to mistake for the navy-and-gray of corporate enterprise or the near-black monoculture of developer tools.

The voice is confident, not loud for its own sake. Big characterful headlines make strong claims ("Charge for your AI product. Today."), and the proof sits right next to them: real code, real product surfaces, rendered as crisp white-paper objects floating on the blue. Motion is choreographed and decisive; entrances are orchestrated, color blocks hand off to each other on scroll, and nothing dribbles in with timid fades.

This system explicitly rejects: the generic SaaS template (purple gradients, identical feature card grids, hero-metric clichés), the crypto/web3 aesthetic (neon glows, glassmorphism-on-dark), corporate enterprise (navy-and-gray, stock photography), and indie-hacker scrappy (emoji, meme energy).

**Key Characteristics:**
- Drenched color strategy: ultramarine carries the surface, white carries the message
- Code-first storytelling on white-paper panels that pop against the blue
- Choreographed motion: orchestrated entrances, scroll-driven color-block handoffs, the capability ticker
- Rounded, confident interactive elements (pill buttons) against sharp color fields
- Premium through precision: typography, spacing, and contrast do the persuading

## 2. Colors

A two-voice palette: ultramarine speaks, white answers. Everything else is a supporting murmur.

### Primary
- **Ultramarine** (oklch(0.42 0.19 264)): the body surface of the brand. Hero, section grounds, the default world the visitor lives in. Hue stays at 264: drifting past ~275 turns it AI-purple, drifting below ~250 turns it corporate navy. Both are failures.
- **Ultramarine Deep** (oklch(0.30 0.14 264)): bands, the capability ticker, footers, pressed states. The same world after dark.

### Neutral
- **Signal White** (oklch(1 0 0)): headlines, primary buttons (white fill, ultramarine text), code panels, product-preview cards. White is an object color here, not just a text color.
- **Blue Mist** (oklch(0.90 0.045 264)): secondary text on ultramarine. Never drop below this lightness for running copy on the blue; body text must hold ≥4.5:1.
- **Paper sections** (white ground, ink oklch(0.15 0 0)): long-form content, docs-flavored sections, and code-heavy passages may invert to white ground with near-black ink. The handoff between blue and white blocks is a scroll moment, not a gradient.

### Named Rules
**The Drench Rule.** The surface IS the color. Do not hedge ultramarine with neutral framing, gray section breaks, or a "safe" white header. When the page isn't blue, it's deliberately, fully white; the cut between the two is the design.

**The Two Blues Rule.** Ultramarine and Ultramarine Deep are the only blues. No third tint, no translucent blue overlays, no blue gradients.

## 3. Typography

**Display Font:** Bricolage Grotesque (characterful grotesque; seed pick, confirm at implementation)
**Body Font:** Hanken Grotesk (seed pick, confirm at implementation)
**Mono Font:** Fragment Mono (code, tickers, technical labels)

**Character:** A grotesque with personality set very large, carried by a plain, highly readable body. The display face brings the campaign energy; the body and mono keep the developer trust. Final families are confirmed during the first build via the font-selection procedure; the pairing axis (characterful display + quiet body + true mono) is the commitment.

### Hierarchy
- **Display** (800, clamp(3rem, 7.5vw, 6rem), 1.0): hero and section-opening claims. Tight but never below -0.03em tracking.
- **Headline** (700, ~2.2rem, 1.1): section heads.
- **Body** (400–500, 1.1–1.2rem, 1.6): running copy, 65–75ch max. Blue Mist on ultramarine, near-black on paper.
- **Mono label** (400, 0.85rem): tickers, file names, terminal chrome, figure annotations.

### Named Rules
**The Claim Rule.** Display type makes one claim per viewport. If a fold needs two headlines, it's two folds.

## 4. Elevation

Flat by doctrine. Depth comes from color blocks meeting each other, not from shadows: blue against deep blue, white objects on blue. White panels (code, product previews) may carry one soft ambient shadow to lift off the blue; nothing else casts anything. No glassmorphism, no blurs-as-decoration, ever.

### Named Rules
**The Poster Rule.** If a surface needs a shadow to be legible, the color relationship is wrong; fix the color, not the shadow.

## 5. Components

Omitted in seed. Components are designed during the first build and captured by the next `/impeccable document` run. Established starting points from the approved board: pill-shaped buttons (white fill + ultramarine text for primary, 1.5px white-outline ghost for secondary), the deep-blue capability ticker, and white code/product panels.

## 6. Do's and Don'ts

### Do:
- **Do** keep the ultramarine surface dominant; commit 30–60%+ of the site to it.
- **Do** put real code and real product UI on white panels; the snippet is the pitch.
- **Do** choreograph motion: orchestrated entrances, scroll-driven color-block handoffs, ease-out-expo curves, full `prefers-reduced-motion` alternatives.
- **Do** hold WCAG AA: ≥4.5:1 body text on every surface, visible focus states, keyboard-complete navigation, accessible forms.
- **Do** write copy with verbs and specific nouns: "Start charging", "Get an API key", never "Learn more".

### Don't:
- **Don't** ship the generic SaaS template: purple gradients, identical icon-card grids, hero-metric blocks, stock 3D illustration.
- **Don't** drift into crypto/web3: neon glows, glassmorphism, dark-mode hype futurism.
- **Don't** go corporate enterprise: navy-and-gray restraint, stock photography, dense jargon.
- **Don't** go indie-hacker scrappy: emoji in UI copy, meme references, Twitter-thread energy.
- **Don't** add a third blue, a blue gradient, or translucent blue overlays (The Two Blues Rule).
- **Don't** use gradient text, side-stripe borders, or tiny uppercase tracked eyebrows above every section.
- **Don't** let ultramarine drift purple (hue > ~275) or navy (hue < ~250).
