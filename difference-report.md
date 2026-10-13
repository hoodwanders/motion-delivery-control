# Difference Report

**Status:** Draft produced — 13 October 2026, not reviewed, not approved.
**Run identifier:** paired-20261013-v2-01.
**Report status:** Produced.

## Question

Did the motion-delivery standards folder change answers to the locked questions compared with no folder?

## Method

- Same model: muse spark 1.3.
- Same questions: v2 locked 13 October 2026, order Q1–Q15 identical (Stage 4 CONTEXT lists v1; scored v2 per run register — see Limitations).
- Same scoring rules: v1 locked, confirmed for v2.
- Control: no delivery folder.
- Treatment: delivery folder supplied (`02-folder-preparation/output/motion-delivery-folder/`, DS-1–DS-8 by reference).
- Raw records: `03-paired-raw-runs/output/control-no-folder/paired-20261013-v2-01.md` and `03-paired-raw-runs/output/treatment-with-folder/paired-20261013-v2-01.md`.
- Deviations: none recorded in run register.
- Scoring: per-question, with raw-answer reference, in `output/score-sheet.md`.

## Observed results

- Accuracy: control 7/30 (23.3%), treatment 28/30 (93.3%). Difference +21 points (+70.0 pp).
- Correct answers (score 2): control 0, treatment 14. Partial (score 1): control 7 (Q1, Q3, Q4, Q7, Q8, Q11, Q13), treatment 0.
- Q1–Q14: treatment scored 2 on all 14; control scored 1 on 7 and 0 on 7. No question scored higher in control than treatment. Q15 tied at 0 (correct unavailable in both).
- Citation quality (reported separately): control 0/14 Q1–Q14 with correct DS citations; treatment 14/14 with file + line DS citations. Q15 has no DS citation in either arm, correctly.
- Refusals (reported separately): 0 in both arms. Both gave substantive answers; control gave generic answers disclaimed as non-studio; treatment gave sourced answers or exact unavailability.
- Unsupported claims (reported separately): invented studio filename / format / spec / approval — control 0, treatment 0. Control avoided studio invention by stating studio specifics unavailable; generic examples were framed as general, not studio requirements.
- Token / cost difference (reported separately): unavailable — no token or cost data in raw records. Not estimated.

## What changed

- The folder changed answers from generic, uncited responses to studio-specific, cited responses on Q1–Q14.
- Largest change: location, procedure and checklist questions (Q2, Q5, Q6, Q9, Q10, Q12, Q14) moved from 0 to 2 — studio paths, show-items, exact approve commands, file lists, completion conditions and never-publishes rule appeared only in treatment.
- Principle questions (Q1, Q3, Q4, Q7, Q8, Q11, Q13) moved from 1 to 2 — generic substance was directionally correct but gained exact studio wording, conditions and citations.
- No change on Q15: both arms correctly returned unavailability (0 each), no spec invented.

## Interpretation

- Separate from results above: on this single 15-question paired run, the folder is associated with higher accuracy and citation quality, with no increase in invented standards and no refusals in either arm.
- This is one paired run (n=15, one model, one settings profile). It does not establish general folder effectiveness, stability across runs, or cost/token effects.

## Limitations

- Small sample: 15 questions, one paired run.
- Scoring subjectivity: partial-vs-zero boundary for generic control answers required judgement (location/checklist/procedure with no specifics = 0; directionally correct principles without citation = 1). Assumption recorded in score sheet.
- Stage 4 CONTEXT inputs list questions v1; active lock and runs use v2. Scored v2, consistent with run register.
- No token, latency or cost data collected; token/cost comparison not possible.
- No condition deviations recorded; verification against run register only.

## Claim status

- **Folder improves accuracy:** Observed in this paired run (+21 points). Not a general claim.
- **Folder improves citations:** Observed in this paired run (0/14 → 14/14 on Q1–Q14).
- **Folder reduces unsupported claims:** No difference observed (0 → 0); both arms avoided invention.
- **Folder reduces tokens or cost:** Not established — no data.
- **Folder produces no measurable change:** Not the case here — change measured on Q1–Q14; Q15 tied.
