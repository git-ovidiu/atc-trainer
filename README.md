# Vector Trainer

**Browser-based practice drills for air traffic controller (ATCO) aptitude tests.**

Vector Trainer is an open-source web app with short, timed exercises that train
the skills ATCO selection tests look for: mental arithmetic under pressure,
spatial orientation, short-term memory, multitasking, and conflict detection.
Each session is scored, and progress is tracked over time so you can see
which skills are improving and which need work.

> Status: **early development** — see [ROADMAP.md](./ROADMAP.md).

## Why

ATCO selection tests are demanding and timed, and good practice tools are
scarce, expensive, or closed. Vector Trainer aims to be a free, offline-capable,
well-tested alternative with **original** exercises (no content copied from
commercial test-prep products).

## Planned drills

| Drill | Skill trained | Description |
|---|---|---|
| **Mental Math** | Numerical speed | Timed arithmetic: speed/distance/time, fuel, altitude differences |
| **Heading Finder** | Spatial orientation | Given a position and a target, pick the correct heading |
| **Relative Position** | Spatial orientation | Rotate the frame of reference: "where is aircraft B from A's point of view?" |
| **Callsign Memory** | Short-term memory | Remember callsigns, flight levels and squawk codes shown briefly |
| **Conflict Watch** | Conflict detection | Aircraft move on a radar-style canvas; flag pairs that will lose separation |
| **Dual Task** | Multitasking | Run a tracking task while answering math or memory prompts |

## Features (planned)

- Configurable difficulty and session length
- Per-drill scoring: accuracy, reaction time, consistency
- Progress history and charts, stored locally in the browser (no accounts, no server)
- Works offline as an installable web app (PWA)
- Keyboard-first controls, accessible color contrast, light and dark themes

## Tech stack

- **TypeScript** + **React** + **Vite**
- **HTML Canvas** for radar-style drills
- **Vitest** for unit tests, **Playwright** for end-to-end tests
- **IndexedDB** for local progress storage
- ESLint + Prettier

## Getting started

> Setup instructions will be added once the app is scaffolded.

```bash
git clone https://github.com/<your-username>/vector-trainer.git
cd vector-trainer
npm install
npm run dev
```

## Project structure (planned)

```
src/
  drills/        # one folder per drill (logic + UI)
  engine/        # timers, scoring, random generators (seeded)
  storage/       # local progress persistence
  components/    # shared UI
  pages/         # home, drill runner, results, history
tests/
  unit/
  e2e/
docs/
```

## Privacy

Vector Trainer collects no personal data. All results stay in your own browser.

## Disclaimer

This is an independent practice tool. It is not affiliated with, endorsed by,
or derived from any official ATCO selection test or commercial test-prep product.

## License

[MIT](./LICENSE) © 2026 Ovidiu Bunghez
