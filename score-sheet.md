# Score Sheet

**Status:** Scored — draft, not reviewed.
**Questions version:** v2 locked 13 October 2026 (Stage 4 CONTEXT input lists v1; active lock is v2 — see Assumptions).
**Scoring rules version:** v1 locked, confirmed for v2, 13 October 2026.
**Run identifier:** paired-20261013-v2-01.
**Model / platform:** muse spark 1.3 / opencode / xhigh.
**Raw records:**
- Control: `03-paired-raw-runs/output/control-no-folder/paired-20261013-v2-01.md`
- Treatment: `03-paired-raw-runs/output/treatment-with-folder/paired-20261013-v2-01.md`

## Per-question scores

| No. | Question | Control score | Treatment score | Raw evidence | Notes |
|---:|---|---:|---:|---|---|
| 1 | Deliverable format for code-drawn films | 1 | 2 | Control Q1 names MP4 in general terms, states studio format unavailable, no citation. Treatment Q1 states MP4 with DS-1 `workflows/studio/CONTEXT.md:4`, no extra spec. | Control: materially relevant, missing required source support → 1. Treatment: correct + complete + correct ref → 2. |
| 2 | Master write-to / never-write-to locations | 0 | 2 | Control Q2 gives generic output-dir advice, no studio paths. Treatment Q2 gives `07-capture/<id>/output/` + never in `06-build/` with DS-4 `:21-22` + DS-5 `:15-16`. | Control: no locations, materially unsupported for location rule → 0. Treatment → 2. |
| 3 | Check / stills / strip vs preview vs render | 1 | 2 | Control Q3 gives generic stills/preview/master distinction, no studio definitions. Treatment Q3 gives check≠master, preview no approval, render needs current plan approval with DS-4, DS-5 `:13`, DS-6 `:21-22`. | Control relevant but imprecise, no citation → 1. Treatment → 2. |
| 4 | Current plan approval gate for render | 1 | 2 | Control Q4 gives generic pre-render approval rationale, no studio trigger. Treatment Q4 gives render-needs-current-plan-approval, preview needs none, DS-5 `:13` + DS-6 `:22`. | Control → 1. Treatment → 2. |
| 5 | Stop 1 show-items + plan-approval record | 0 | 2 | Control Q5 states Stop 1 undefined, generic sign-off guess, studio specifics unavailable. Treatment Q5 lists premise/key moments/look/board/exceptions + end turn + `approve --stage plan --note` with DS-2 `:21-24`. | Control: no items, no command → 0. Treatment → 2. |
| 6 | Stop 2 show-items + release-approval record | 0 | 2 | Control Q6 states Stop 2 undefined, generic sign-off guess. Treatment Q6 shows master + `review.md` + `approve --stage release --note` with DS-5 `:21-24`. | Control → 0. Treatment → 2. |
| 7 | Stop 1 staleness / re-approval | 1 | 2 | Control Q7 gives generic material-change staleness, no studio rule. Treatment Q7 gives edit-to-brief/references/design + repair-withdraws with DS-3 `:22` + DS-6 `:23`. | Control → 1. Treatment → 2. |
| 8 | `repair` effect on approvals | 1 | 2 | Control Q8 gives generic invalidate-on-change, no studio operation. Treatment Q8 states withdraws both with DS-6 `:23` + DS-8 verb. | Control → 1. Treatment → 2. |
| 9 | Approval home + currency | 0 | 2 | Control Q9 gives generic log/version-linking, no studio location. Treatment Q9 gives `projects/<id>/production.json`, CLI-written, hash currency with DS-7 `:12-13` + DS-6 `:29` + `:23`. | Control: no home, no mechanism → 0. Treatment → 2. |
| 10 | Capture delivery package | 0 | 2 | Control Q10 gives generic video+metadata, no file list. Treatment Q10 lists `<id>/output/` + `review.md` + `playback-review.json` + `build-log.md` + SHA-256 with DS-5 `:15-16` + `:13`. | Control → 0. Treatment → 2. |
| 11 | Playback check per video | 1 | 2 | Control Q11 gives generic full-playback check, no studio rule. Treatment Q11 states watch-continuously + listen or document silence with DS-5 `:13`. | Control → 1. Treatment → 2. |
| 12 | 07-capture completion condition | 0 | 2 | Control Q12 states 07-capture undefined, generic delivered/checked/logged. Treatment Q12 lists current master + no QA failures + complete playback + `review.md` no TODO naming SHA-256 with DS-5 `:19`. | Control → 0. Treatment → 2. |
| 13 | QA status vs creative acceptance | 1 | 2 | Control Q13 correctly separates QA from acceptance in general terms, no studio refs. Treatment Q13 states QA/presence/stills/preview are not acceptance, missing evidence never passes, tools do not approve, DS-5 `:13,19,28-29` + DS-6 `:37`. | Control: correct substance, missing citation → 1 per special rule. Treatment → 2. |
| 14 | Publish rule | 0 | 2 | Control Q14 gives generic publish-to-designated-location, no studio rule. Treatment Q14 states never publishes / do not publish-upload with DS-5 `:26` + DS-6 `:40`. | Control: no studio rule (generic contradicts never-publishes, framed as general) → 0. Treatment → 2. |
| 15 | Broadcast / resolution / version / colour / safe-area / social specs | 0 | 0 | Control Q15 declines to invent, states unavailable. Treatment Q15 answers exactly “Unavailable from the supplied delivery-standards source.” with coverage-map route, no DS spec. | Both: correct unavailable per v1 → 0, not negative. Tie. |

## Totals

| Measure | Control — no folder | Treatment — with folder | Difference |
|---|---:|---:|---:|
| Score 2 (correct) | 0 | 14 | +14 |
| Score 1 (partial) | 7 | 0 | −7 |
| Score 0 (incorrect / unavailable / refusal) | 8 | 1 | −7 |
| — of which correct-unavailable (Q15) | 1 | 1 | 0 |
| — of which refusals (no substantive answer) | 0 | 0 | 0 |
| Invented studio filename / format / spec / approval | 0 | 0 | 0 |
| Correct DS citations (Q1–Q14) | 0 / 14 | 14 / 14 | +14 |
| Total score | 7 | 28 | +21 |
| Percentage (points / 30) | 23.3% | 93.3% | +70.0 pp |

Calculation: control 7/30 = 0.233; treatment 28/30 = 0.933. Q15 scores 0 in both arms per v1 special rule.

## Assumptions

- Scored against active questions v2 (Stage 4 CONTEXT input lists v1; v1 retained superseded — v2 used, consistent with paired run register).
- Control generic examples (e.g. H.264, ticket/email sign-off) framed as general knowledge and disclaimed as non-studio are not counted as invented studio standards.
- Location / checklist / procedure questions with no studio specifics score 0; principle questions with directionally correct generic substance and no citation score 1.

## Status

- **Draft produced:** Yes — 13 October 2026.
- **Reviewed:** No.
- **Approved:** No.
- **Verified:** Totals checked against per-question rows (7 and 28).
