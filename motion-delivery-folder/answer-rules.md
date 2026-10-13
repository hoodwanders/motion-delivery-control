# Answer Rules — questions v2

**Status:** Built 13 October 2026.

## General rules

1. Check `coverage-map.md` first; use the DS route for the question number.
2. Resolve DS IDs via `sources/studio-source-pointer.md`; cite the file and line/section.
3. Quote or precisely reference the supporting rule; do not paraphrase away conditions (e.g. “current” plan approval, “continuously” watched, “their words” note).
4. Distinguish source fact, procedure step, and interpretation.
5. If DS sections conflict, report both and identify the conflict.
6. If the map says explicit unavailability (Q15), answer exactly: “Unavailable from the supplied delivery-standards source.” Name the missing spec type; do not fill it from general knowledge.
7. Do not use outside knowledge to fill a source gap. MP4 is the only format claim; no resolution, frame rate, codec, colour, naming-pattern, version-number, or broadcast claims exist.
8. Do not provide a longer answer than the question requires.
9. Scoring match (v1): a correct answer with missing or wrong citation scores at most 1; any invented filename, format, spec, or approval rule scores 0.

## Question routes

| Questions | Route |
|---|---|
| Q1 format | State MP4 per DS-1; add no broadcast claim |
| Q2 locations | State write-to and never-write-to per DS-4/DS-5 with paths |
| Q3 three-way distinction | State check != master (DS-4); preview = review copy, no approval; render = master + QA, needs current plan approval (DS-5) |
| Q4 render gate | State current-plan-approval requirement per DS-5:13 |
| Q5 Stop 1 | List show-items + end-turn + exact approve command per DS-2 |
| Q6 Stop 2 | List show-items + end-turn + exact approve command per DS-5:21-24 |
| Q7 staleness | State DS-3 edit rule + DS-6 repair-withdraws rule |
| Q8 repair | State withdraws both approvals per DS-6 |
| Q9 home + currency | State `production.json` home per DS-7 + hash-currency per DS-6 |
| Q10 package | List the four artefacts + SHA-256 per DS-5:15-16 |
| Q11 playback | State watch-continuously + listen-or-document-silence per DS-5:13 |
| Q12 completion | List the four conditions per DS-5:19 |
| Q13 QA vs acceptance | State QA / presence / stills / preview are not acceptance; missing evidence never passes; tools do not approve (DS-5 + DS-6) |
| Q14 publish | State never-publishes / do-not-publish-upload (DS-5:26, DS-6:40) |
| Q15 out-of-scope specs | State unavailable; identify the missing spec type; stop |
