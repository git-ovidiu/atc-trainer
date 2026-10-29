# Roadmap

Milestones are ordered; items inside a milestone can be done in any order.
Each checkbox is roughly one focused work session.

## M0 — Foundation
- [ ] Scaffold Vite + React + TypeScript project
- [ ] Set up ESLint, Prettier, Vitest, Playwright
- [ ] GitHub Actions CI: lint, type-check, unit tests on every push
- [ ] App shell: routing, layout, light/dark theme
- [ ] Seeded random number generator (reproducible drills for testing)

## M1 — Drill engine
- [ ] Generic drill runner: countdown, timer, question loop, end screen
- [ ] Scoring model: accuracy, mean reaction time, consistency
- [ ] Difficulty settings (easy / normal / hard / custom)
- [ ] Keyboard input handling shared across drills

## M2 — First drills
- [ ] **Mental Math** — arithmetic generator with aviation-flavored problems
- [ ] **Heading Finder** — compass rendering + heading calculation
- [ ] **Callsign Memory** — show/hide sequence, recall input
- [ ] Unit tests for every generator and scoring function

## M3 — Progress tracking
- [ ] Persist session results in IndexedDB
- [ ] History page with per-drill charts
- [ ] Personal bests and streaks
- [ ] Export / import results as JSON (backup)

## M4 — Radar drills
- [ ] Canvas radar view: aircraft movement, labels, range rings
- [ ] **Conflict Watch** — trajectory prediction and separation checks
- [ ] **Relative Position** — rotating frame-of-reference drill
- [ ] Performance pass: steady 60 fps on mid-range laptops

## M5 — Multitasking
- [ ] **Dual Task** — tracking task + interrupting prompts
- [ ] Combined "exam simulation" mode chaining several drills

## M6 — Polish & release
- [ ] PWA: offline support, installable on desktop and tablet
- [ ] Accessibility audit (keyboard, contrast, screen reader labels)
- [ ] Playwright end-to-end tests for each drill
- [ ] Documentation: drill descriptions, contributing guide
- [ ] v1.0 release and deploy to GitHub Pages

## Ideas / later
- Adaptive difficulty that adjusts to the user's recent performance
- Sound cues and simulated radio callouts (text-to-speech)
- Localization (English, Romanian)
