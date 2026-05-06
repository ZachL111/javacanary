# javacanary

`javacanary` keeps a focused Java implementation around reliability. The project goal is to debounce health checks and explain readiness state.

## Purpose

The point is to make a small domain rule concrete enough that a reader can change it and immediately see what broke.

## Javacanary Review Notes

For a quick review, compare `failure width` with `budget pressure` before reading the middle cases.

## What Is Covered

- `fixtures/domain_review.csv` adds cases for budget pressure and failure width.
- `metadata/domain-review.json` records the same cases in structured form.
- `config/review-profile.json` captures the read order and the two review questions.
- `examples/javacanary-walkthrough.md` walks through the case spread.
- The Java code includes a review path for `failure width` and `budget pressure`.
- `docs/field-notes.md` explains the strongest and weakest cases.

## Implementation Notes

The fixture data drives the tests. The code stays thin, while `metadata/domain-review.json` and `config/review-profile.json` explain what each case is meant to protect.

The added Java path is deliberately direct, with fixtures doing most of the explaining.

## Command

```powershell
powershell -NoProfile -ExecutionPolicy Bypass -File scripts/verify.ps1
```

## Audit Path

That command is also the regression path. It verifies the domain cases and catches mismatches between the CSV, metadata, and code.

## Limits

The repository is intentionally scoped to local checks. I would expand it by adding adversarial fixtures before adding features.
