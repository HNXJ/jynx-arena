# todo stack

Top = next. Gate: `npm ci && npm run build && npm run lint`.

- T-1 Add a test runner and a first test (`tests/` holds only `.gitkeep`; `package.json` has no `test` script). Closes when: `npm test` exits 0 and reports at least 1 passed. Blocked by: none.
- T-2 Split the main bundle; `npm run build` warns a chunk exceeds 500 kB. Closes when: `npm run build` prints no chunk-size warning. Blocked by: none.
- T-3 Triage open issues #1 to #5. Closes when: `gh issue list -R HNXJ/jynx-arena --state open --json number -q length` prints 0. Blocked by: none.
