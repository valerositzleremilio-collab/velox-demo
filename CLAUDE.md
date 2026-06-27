# VELOX — Project Context for Claude Code

## What this is
Single-page cinematic landing page for fictional luxury sports car brand VELOX.
Built by Oddomode (oddomode.de). Demo site to showcase Oddomode's capabilities.

## Design Tokens
- Background: #0D0D0B (near-black)
- Accent: #C8F135 (electric lime)
- Text: #F0EDE6 (warm cream)
- White: #ffffff
- Font: Inter 900 for headlines, Inter 400 for body

## Tech Stack
- Pure HTML/CSS/JS — single file (index.html)
- GSAP 3.12.5 + ScrollTrigger via CDN
- NO Lenis (removed — was causing bugs)
- NO frameworks, NO npm
- Hosted: GitHub → Vercel (auto-deploy on push)

## Files in this folder
- index.html — the entire website
- clip1.mp4 — chase shot (hero scroll video)
- clip2.mp4 — wheel spin (reveal section)
- clip3.mp4 — front attack (reveal section)
- bild3-seite.png — dark side silhouette
- bild5-silhouette.png — outdoor side profile

## Current known bugs
1. Lenis conflicts with ScrollTrigger — REMOVE Lenis
2. Section heights too tall — reduce all vh values
3. Colors too dull — increase contrast and vibrancy
4. Hero video not loading — needs autoplay + ScrollTrigger fix
5. gsap.set must run BEFORE gsap.timeline in preloader

## Reference: landonnorris.com
- High contrast, zero dullness
- Electric accent used aggressively
- Typography slams — y:80 entrances, scale from 0.6
- Speed and kinetic energy in every transition
- Tight spacing — not 300vh of empty black

## Deploy command (run after every change)
git add . && git commit -m "fix: [describe change]" && git push

## Rules
- Never add npm, webpack, or any build tool
- Never add frameworks (no React, no Vue)
- Always use CSS custom properties (var(--black) etc)
- Every section needs a comment header
- After changes: always run the deploy command
