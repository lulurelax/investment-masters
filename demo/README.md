# Investment Masters demos

These examples are **synthetic documentation fixtures**. They show the shape of
a careful methodology comparison; they are not current holdings, signals,
recommendations or claims about what any investor currently believes.

| Fixture | Purpose |
|---|---|
| [`compare-buffett-marks.md`](compare-buffett-marks.md) | Compare two lenses without pretending the result is a forecast |
| [`masters-preview.json`](masters-preview.json) | Machine-readable discovery view for the four defaults and all 15 profiles |

For current claims, ask the agent to identify the dated source first. A 13F
question must name the reporting entity, filing period and publication date;
this repository does not fetch or refresh holdings automatically.

## Every profile has a real-source case

[`masters-cases.json`](masters-cases.json) contains one reproducible case for
each of the 15 profiles. The cases use current public source pages or dated
filings at run time, and show the question, evidence boundary and expected
output. They do not invent current holdings or imply endorsement.

Inspect one case:

```bash
jq '.cases[] | select(.profile == "buffett")' demo/masters-cases.json
```
