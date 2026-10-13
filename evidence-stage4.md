# Stage 4 evidence

## Source facts

- Run: paired-20261013-v2-01, muse spark 1.3 / opencode / xhigh, questions v2 Q1–Q15, scoring v1. Run register: `03-paired-raw-runs/output/run-register.md`.
- Control raw: `03-paired-raw-runs/output/control-no-folder/paired-20261013-v2-01.md` (35 lines, generic answers, no DS citations, studio specifics stated unavailable).
- Treatment raw: `03-paired-raw-runs/output/treatment-with-folder/paired-20261013-v2-01.md` (106 lines incl. headers, DS-1–DS-8 file+line citations, Q15 exact unavailability).
- Locked questions: `01-source-and-question-lock/output/questions-v2.md` (v2, Q1–Q14 routed to DS, Q15 explicit unavailability).
- Locked scoring: `01-source-and-question-lock/output/scoring-rules.md` (2/1/0 scale, missing/wrong citation caps at 1, invention scores 0, correct unavailable scores 0, max 30).
- Folder: `02-folder-preparation/output/motion-delivery-folder/` (CLAUDE.md + CONTEXT.md + coverage-map.md + answer-rules.md + `sources/studio-source-pointer.md` resolving DS-1–DS-8 by reference).
- Scores: control 7/30 (23.3%), treatment 28/30 (93.3%), per-question evidence in `output/score-sheet.md`. Claims reconcile with score sheet.

## Source defaults

- None used for scoring. Generic control content scored as partial only where directionally correct; no general-knowledge defaults asserted as studio standards.

## Derivations

- Accuracy, citation quality, refusals, unsupported claims, tokens/cost reported separately in `output/difference-report.md` (accuracy +21, citations 0/14 → 14/14, refusals 0/0, inventions 0/0, tokens unavailable).
- Interpretation separated from observed results; single-run limit stated; no general effectiveness claimed.

## Assumptions

- Scored v2 (active lock); Stage 4 CONTEXT input line lists v1 — recorded in score sheet and report, not silently resolved.
- Control generic examples disclaimed as non-studio are not counted as invented studio standards.
- Location/checklist/procedure with no studio specifics = 0; directionally correct principles without citation = 1.

## Gaps

- Token, latency and cost data: unavailable (not in raw records).
- HG review and approval: pending. Decision status remains Not reviewed.
- Reproducibility: single run; re-run stability untested.
