# Coverage Map — questions v2

**Status:** Fixed 14 October 2026 — routes now to vendored `sources/vendor-studio/` (byte-identical to DS-1–DS-8 approved 13 October 2026).
**Source:** DS-1–DS-8 vendored via `sources/studio-source-pointer.md` + `sources/vendor-studio/`.
**Questions:** `../../01-source-and-question-lock/output/questions-v2.md` (locked).  
**Scoring:** `../../01-source-and-question-lock/output/scoring-rules.md` v1.

| Q | Topic | Covered | Source reference | Notes |
|---|---|---|---|---|
| 1 | Deliverable format | Yes | DS-1 (`sources/vendor-studio/workflows/studio/CONTEXT.md:4`) | MP4; no broadcast spec claimed |
| 2 | Master write location | Yes | DS-4 (`sources/vendor-studio/workflows/studio/06-build/CONTEXT.md:21-22`), DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:15-16`) | `07-capture/<id>/output/`; never in `06-build/` |
| 3 | Check / preview / master distinction | Yes | DS-4 (check is not a master), DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:13` preview vs render), DS-6 CLI verbs | Preview needs no approval; render needs current plan approval |
| 4 | Plan-approval gate for render | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:13`) | Current plan approval required |
| 5 | Stop 1 show + record | Yes | DS-2 (`sources/vendor-studio/workflows/studio/03-design/CONTEXT.md:21-24`) | Premise/key moments/look/board/exceptions; `approve --stage plan --note "<their words>"` |
| 6 | Stop 2 show + record | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:21-24`) | Master + `review.md`; `approve --stage release --note "<their words>"` |
| 7 | Stop 1 staleness | Yes | DS-3 (`sources/vendor-studio/workflows/studio/04-shot-plan/CONTEXT.md:22`), DS-6 (repair withdraws both) | Edit to brief/references/design or repair → re-approval |
| 8 | Repair effect | Yes | DS-6 (`sources/vendor-studio/workflows/studio/cli/tools/CONTEXT.md:22-23`) | Withdraws plan and release approvals |
| 9 | Approval home + currency | Yes | DS-6 + DS-7 (`projects/<id>/production.json`; current only while hashes match) | CLI-written; pointers only in log |
| 10 | Capture delivery package | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:15-16`) | `<id>/output/` + `review.md` + `playback-review.json` + `build-log.md`, each video SHA-256 |
| 11 | Playback check | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:13`) | Watch continuously + listen, or document intentional silence |
| 12 | 07-capture completion | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:19`) | Current master, no QA failures, complete playback, `review.md` no TODO naming each SHA-256 |
| 13 | QA vs acceptance | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:19,29`), DS-6 (`sources/vendor-studio/workflows/studio/cli/tools/CONTEXT.md:37`) | QA / file presence / stills / preview are not acceptance; missing evidence never passes; tools do not approve |
| 14 | Publish rule | Yes | DS-5 (`sources/vendor-studio/workflows/studio/07-capture/CONTEXT.md:26`), DS-6 (`sources/vendor-studio/workflows/studio/cli/tools/CONTEXT.md:40`) | Never publishes; do not publish/upload |
| 15 | Broadcast / resolution / version / colour / safe-area / social specs | Explicit unavailability | None in DS-1–DS-8 | Correct answer: “Unavailable from the supplied delivery-standards source.” |

## Verification

- 15/15 questions have a source route or explicit unavailability route.
- No `Unresolved` remains in this map.
- No broadcast, resolution, version-number, colour, safe-area, or social spec invented.
