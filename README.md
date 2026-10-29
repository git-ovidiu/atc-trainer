# Vector Trainer

*Practice drills for air traffic controller aptitude tests, right in your browser.*

ATCO selection tests are demanding and timed, and good practice tools are
scarce, expensive, or closed. Vector Trainer is meant to be the free,
open-source alternative: short timed exercises for the skills these tests look
for — mental arithmetic under pressure, spatial orientation, short-term memory,
multitasking and conflict detection. Every session gets a score, and your
progress is tracked over time so you can see which skills are improving and
which still need work.

All exercises are **original**; nothing is copied from commercial test-prep
products. It is designed to work offline and to be well tested.

**Project status:** early development. What's coming next is in the
[roadmap](./ROADMAP.md).

---

## The drills

### Mental Math
*Trains numerical speed.* Timed arithmetic built around aviation problems:
speed/distance/time, fuel, and altitude differences.

### Heading Finder
*Trains spatial orientation.* You get a position and a target and have to pick
the correct heading.

### Relative Position
*Trains spatial orientation.* Rotate the frame of reference and answer
questions like "where is aircraft B from A's point of view?"

### Callsign Memory
*Trains short-term memory.* Callsigns, flight levels and squawk codes flash on
screen briefly — then you recall them.

### Conflict Watch
*Trains conflict detection.* Aircraft move across a radar-style canvas; flag
the pairs that are going to lose separation.

### Dual Task
*Trains multitasking.* Keep a tracking task going while answering math or
memory prompts.

## What else is planned

You'll be able to set the difficulty and the length of a session. Each drill
reports accuracy, reaction time and consistency. Your history and charts live
in your own browser — there are no accounts and no server. The app can be
installed as a PWA and keeps working offline. Controls are keyboard-first, with
accessible color contrast and both a light and a dark theme.

## Under the hood

Written in TypeScript with React and Vite. Radar-style drills are drawn on an
HTML canvas, and progress is saved in IndexedDB. Unit tests run on Vitest,
end-to-end tests on Playwright, and the code is kept tidy with ESLint and
Prettier.

## Running it locally

Detailed setup steps will follow once the app is scaffolded. The plan is:

```bash
git clone https://github.com/git-ovidiu/atc-trainer.git
cd atc-trainer
npm install
npm run dev
```

## How the code will be organized

- `src/drills/` — one folder per drill, holding its logic and its UI
- `src/engine/` — timers, scoring and seeded random generators
- `src/storage/` — saving progress locally
- `src/components/` — UI pieces shared between drills
- `src/pages/` — home, drill runner, results and history screens
- `tests/unit/` and `tests/e2e/` — the two test suites
- `docs/` — documentation

## A note on privacy

No personal data is collected. Your results never leave your browser.

## Not an official test

Vector Trainer is an independent practice tool. It isn't affiliated with,
endorsed by, or derived from any official ATCO selection test or commercial
test-prep product.

---

Released under the [MIT License](./LICENSE). Copyright © 2026 Ovidiu Bunghez.
