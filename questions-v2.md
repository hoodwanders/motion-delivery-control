# Locked Question Set — v2 (studio-native)

**Status:** Locked.  
**Version:** v2.
**Question count:** 15.  
**Supersedes:** v1 (v1 stays locked; runs on v2 require fresh paired runs).  
**Source:** DS-1–DS-8 in `delivery-standards-source-index.md` (approved 13 October 2026).  
**Scoring:** scoring-rules v1 (confirmed applies to v2, 13 October 2026).
**Approved by HG:** Yes — chat, 13 October 2026.

## Rules

- Both arms receive these questions in this order.
- Any change after lock creates v3 and requires new paired runs.
- Answers must cite the DS source where applicable.
- If the source does not answer a question, the correct response is: “Unavailable from the supplied delivery-standards source.”

## Questions

| No. | Question | Answer type | Source route |
|---:|---|---|---|
| 1 | What deliverable format does the studio produce for code-drawn films? | Fact plus citation | DS-1 (`workflows/studio/CONTEXT.md:4`) |
| 2 | Where must master renders be written, and where must they not be written? | Location rule plus citation | DS-4 (`06-build/CONTEXT.md:15-22`), DS-5 (`07-capture/CONTEXT.md:15-16`) |
| 3 | What is the difference between a check / stills / strip, a preview, and a render (master)? | Distinction plus citation | DS-4 (check is not a master), DS-5 (preview = review copy no approval; render = master), DS-6 CLI verbs |
| 4 | When is a current plan approval required before a render? | Decision rule plus citation | DS-5 (`07-capture/CONTEXT.md:13` — render needs current plan approval) |
| 5 | What must be shown at Stop 1, and how is plan approval recorded? | Procedure plus citation | DS-2 (`03-design/CONTEXT.md:21-24`) |
| 6 | What must be shown at Stop 2, and how is release approval recorded? | Procedure plus citation | DS-5 (`07-capture/CONTEXT.md:21-24`) |
| 7 | When does Stop 1 become stale and require re-approval? | Decision rule plus citation | DS-3 (`04-shot-plan/CONTEXT.md:22`), DS-6 (repair withdraws both) |
| 8 | What does `repair` do to existing plan and release approvals? | Rule plus citation | DS-6 (`cli/tools/CONTEXT.md:22-23`) |
| 9 | Where do approvals live, and what keeps them current? | Fact plus citation | DS-6 + DS-7 (`projects/<id>/production.json`; current only while hashes match) |
| 10 | What files constitute a complete capture delivery for one run? | Checklist plus citation | DS-5 (`<id>/output/` + `review.md` + `playback-review.json` + `build-log.md` with each video SHA-256) |
| 11 | What playback check is required for each delivered video? | Rule plus citation | DS-5 (watch continuously + listen, or document intentional silence) |
| 12 | What is the completion condition for 07-capture? | Checklist plus citation | DS-5 (current master, no QA failures, complete playback record, `review.md` no TODO naming each SHA-256) |
| 13 | What is the relationship between QA status and creative acceptance? | Rule plus citation | DS-5 + DS-6 (QA is not acceptance; file presence is not acceptance; missing evidence never passes; tools do not approve films) |
| 14 | What is the studio's publish rule? | Rule plus citation | DS-5 (`07-capture/CONTEXT.md:26` — never publishes), DS-6 (do not publish/upload) |
| 15 | What is the correct response if asked for a broadcast specification, resolution / frame rate, version-number scheme, colour-management rule, safe-area rule, or social-cutdown spec? | Explicit unavailability | None in DS-1–DS-8 — answer: “Unavailable from the supplied delivery-standards source.” |

## Coverage note

- Q1–Q14: answerable or partly answerable from DS-1–DS-8.
- Q15: correctly unavailable — tests refusal behaviour; scores 0 in both arms per scoring-rules v1.
- No broadcast, resolution, version-number, colour, safe-area, or social specs invented. Gaps preserved.

## Status

- **Template prepared:** Yes.
- **Locked:** Yes — v2.
- **Approved by HG:** Yes — chat, 13 October 2026.
