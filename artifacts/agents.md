# agents

Frontend: map, quests, players, leaderboard, replays. One client of the versioned API.

## Layout

- `src/` React + TypeScript (Vite, Tailwind): `registry/`, `components/`, `api/client.ts`, `data/`.
- `public/` static assets. `schemas/`, `tournaments/`, `tests/` empty. `artifacts/archive/` retired files.
- Config via `.env` copied from `.env.example`; never commit `.env`.

## Build and test

```
npm ci
npm run build
npm run lint
npm run dev     # local server
```

Gate: `npm run build && npm run lint`, both rc 0. Root layout check (needs a jynx-engine checkout): `python <jynx-engine>/src/scripts/check_shared_root.py .` prints `OK`.

## Git

- Work on `_temp_<name>` branches; PR to `main`. No direct push to `main`.
- Stage exact paths; never `git add .` or `-A`.
- Never commit `.env`, tokens or keys.
