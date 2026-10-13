# Motion Delivery Control — Competition Submission

Paired test of whether a motion-delivery standards folder changes answers to fixed client-delivery questions.

## Result (one paired run)

- Run: `paired-20261013-v2-01`, 13 October 2026 (UTC).
- Model / platform: muse spark 1.3 / opencode / xhigh.
- Questions: v2 locked (15 questions, order Q1–Q15 identical in both arms).
- Scoring: v1 locked (2/1/0 scale, max 30; correct unavailable scores 0).
- Control (no folder): 7/30 (23.3%).
- Treatment (with folder): 28/30 (93.3%).
- Difference: +21 points (+70.0 pp). Q1–Q14 all moved up; Q15 tied at 0 (correct unavailability in both).
- Citations Q1–Q14: control 0/14, treatment 14/14 with file + line.
- Refusals: 0 both arms. Invented studio standards: 0 both arms.
- Tokens / cost: not measured (no data in raw records).
- Deviations: none recorded.

Status: Stage 4 draft, not reviewed, not approved. This submission reports one paired run only; it does not claim general effectiveness.

## How judges inspect this run

1. Read `questions-v2.md` (locked set) and `scoring-rules.md` (locked scale).
2. Read `delivery-standards-source-index.md` (DS-1–DS-8 authority) and `SOURCE-NOTE.md` (source dependency).
3. Read the folder: `motion-delivery-folder/` (`CLAUDE.md`, `CONTEXT.md`, `coverage-map.md`, `answer-rules.md`, `sources/studio-source-pointer.md`).
4. Read `run-register.md` (run identifier, order, storage, deviations).
5. Read both raws unedited: `control-no-folder-paired-20261013-v2-01.md`, `treatment-with-folder-paired-20261013-v2-01.md`.
6. Check `score-sheet.md` (per-question scores with raw evidence) — verify totals: control 7, treatment 28.
7. Read `difference-report.md` (accuracy, citations, refusals, unsupported claims, tokens reported separately) and `evidence-stage4.md` (provenance, assumptions, gaps).

## File map

| File | Origin |
|---|---|
| `motion-delivery-folder/` | Copy of `02-folder-preparation/output/motion-delivery-folder/` |
| `questions-v2.md` | Copy of `01-source-and-question-lock/output/questions-v2.md` |
| `scoring-rules.md` | Copy of `01-source-and-question-lock/output/scoring-rules.md` |
| `delivery-standards-source-index.md` | Copy of `01-source-and-question-lock/output/delivery-standards-source-index.md` |
| `run-register.md` | Copy of `03-paired-raw-runs/output/run-register.md` |
| `control-no-folder-paired-20261013-v2-01.md` | Copy of `03-paired-raw-runs/output/control-no-folder/paired-20261013-v2-01.md` (unedited) |
| `treatment-with-folder-paired-20261013-v2-01.md` | Copy of `03-paired-raw-runs/output/treatment-with-folder/paired-20261013-v2-01.md` (unedited) |
| `score-sheet.md` | Copy of `04-comparison-and-report/output/score-sheet.md` |
| `difference-report.md` | Copy of `04-comparison-and-report/output/difference-report.md` |
| `evidence-stage4.md` | Copy of `04-comparison-and-report/references/evidence.md` |

Raw files are byte copies; they were not edited for submission. Absolute local paths inside citations are preserved as evidence (see `SOURCE-NOTE.md`).
