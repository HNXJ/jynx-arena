# gamma-arena

Read-only frontend client of the versioned API and event stream.

Proposed future name: **jynx-arena** (proposal, not renamed yet)

## Place in the 7-repo layout

Plane: **ARENA**. See [HNXJ/jynx-arena](https://github.com/HNXJ/jynx-arena) and its [architecture](https://github.com/HNXJ/jynx-arena/blob/main/docs/protocol/ARCHITECTURE.md) (ARENA, RULES, SCIENCE, LAB, ENGINE, JUDGE, WORLD). The current jynx-arena runtime is proposed to become **jynx-engine**; **jynx-world** (event ledger, projections) is a new proposed repo.

## Holds today

- React + TypeScript + Vite app under `src/` (components, api, view-models, registry).
- `docs/ARCHITECTURE.md`, `docs/issue-drafts/`, `MIGRATION.md`.
- `artifacts/generated/`.

## Shared root layout (target, not yet applied)

`artifacts/`, `docs/`, `src/`, `schemas/`, `tests/`, `tournaments/`, `README.md` — see [SHARED_ROOT_LAYOUT](https://github.com/HNXJ/jynx-arena/blob/main/docs/protocol/SHARED_ROOT_LAYOUT.md).

## Truth safety

A Judge PASS means a submission met a rubric under a protocol version; it is not scientific truth.

Ignore rules: `.DS_Store`, `*.npy`, `*.mat` are ignored; `*.html` is not (frontend project).
