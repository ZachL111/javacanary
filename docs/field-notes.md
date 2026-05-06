# Field Notes

`javacanary` is easiest to review by starting with the fixture, not the prose.

The domain cases cover `budget pressure`, `failure width`, `recovery gap`, and `runbook drift`. They sit beside the smaller starter fixture so the project has both a compact scoring check and a domain-flavored review check.

`stress` is the strongest case at 238 on `failure width`. `baseline` is the cautious anchor at 167 on `budget pressure`.

The extra check gives the repository a behavior path that can fail for a domain reason, not only a syntax reason.
