# Review Journal

The repository goal stays the same: debounce health checks and explain readiness state. This note explains the added review angle.

The local checks classify each case as `ship`, `watch`, or `hold`. That gives the project a small review vocabulary that matches its reliability focus without claiming live deployment or external usage.

## Cases

- `baseline`: `budget pressure`, score 167, lane `ship`
- `stress`: `failure width`, score 238, lane `ship`
- `edge`: `recovery gap`, score 217, lane `ship`
- `recovery`: `runbook drift`, score 227, lane `ship`
- `stale`: `budget pressure`, score 220, lane `ship`

## Note

The repository should be understandable without pretending it is larger than it is.
