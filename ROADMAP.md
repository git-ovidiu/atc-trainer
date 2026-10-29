# Vector Trainer — release plan

The project grows one release at a time. Every release builds on the one
before it, so they ship in order; the tasks within a release can be picked up
in any order. A single task is sized for one focused work session.

---

### v0.1 · The groundwork
Get a solid, tested project skeleton in place.

- [ ] Scaffold the project with Vite, React and TypeScript
- [ ] Add ESLint, Prettier, Vitest and Playwright
- [ ] GitHub Actions CI running lint, type-check and unit tests on every push
- [ ] Build the app shell: routing, layout, light/dark theme
- [ ] Write a seeded random number generator so drills are reproducible in tests

### v0.2 · A drill engine
One shared engine that every drill runs on.

- [ ] Generic drill runner — countdown, timer, question loop, end screen
- [ ] Scoring model covering accuracy, mean reaction time and consistency
- [ ] Difficulty settings: easy, normal, hard and custom
- [ ] Shared keyboard input handling for all drills

### v0.3 · The first three drills
- [ ] Mental Math, with an aviation-flavored arithmetic generator
- [ ] Heading Finder, with compass rendering and heading calculation
- [ ] Callsign Memory, with a show/hide sequence and recall input
- [ ] Unit tests for every generator and every scoring function

### v0.4 · Remembering progress
- [ ] Save session results to IndexedDB
- [ ] History page with charts for each drill
- [ ] Personal bests and streaks
- [ ] Back up and restore results as JSON (export / import)

### v0.5 · On the radar
- [ ] Radar view on canvas — moving aircraft, labels, range rings
- [ ] Conflict Watch, using trajectory prediction and separation checks
- [ ] Relative Position, the rotating frame-of-reference drill
- [ ] Performance pass to hold 60 fps on mid-range laptops

### v0.6 · Doing two things at once
- [ ] Dual Task — a tracking task interrupted by prompts
- [ ] Exam simulation mode that chains several drills together

### v1.0 · Ready for real use
- [ ] PWA support: works offline, installable on desktop and tablet
- [ ] Accessibility audit — keyboard, contrast, screen reader labels
- [ ] Playwright end-to-end test for each drill
- [ ] Docs: a description of every drill and a contributing guide
- [ ] Tag v1.0 and deploy to GitHub Pages

---

**Someday, maybe:** difficulty that adapts to your recent results · sound cues
and simulated radio callouts with text-to-speech · English and Romanian
translations.
