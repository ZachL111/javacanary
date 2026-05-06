# Javacanary Walkthrough

I use this file as a small checklist before changing the Java implementation.

| Case | Focus | Score | Lane |
| --- | --- | ---: | --- |
| baseline | budget pressure | 167 | ship |
| stress | failure width | 238 | ship |
| edge | recovery gap | 217 | ship |
| recovery | runbook drift | 227 | ship |
| stale | budget pressure | 220 | ship |

Start with `stress` and `baseline`. They create the widest contrast in this repository's fixture set, which makes them better review anchors than the middle cases.

If `baseline` becomes less cautious without a clear reason, I would inspect the drag input first.
