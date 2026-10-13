# Treatment raw run — paired-20261013-v2-01
**Arm:** treatment-with-folder
**Model:** muse spark 1.3
**Folder:** 02-folder-preparation/output/motion-delivery-folder/
**Questions:** v2, order Q1-Q15
**Date (UTC):** 13 October 2026

## Q1
What deliverable format does the studio produce for code-drawn films?

The studio produces code-drawn films captured to MP4.

Citations:
- DS-1 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\CONTEXT.md:4` — "The animation workflow. Code-drawn films, captured to MP4."
- No broadcast, resolution, frame rate, codec, colour, or other format specification is stated in DS-1–DS-8.

## Q2
Where must master renders be written, and where must they not be written?

Master renders must be written to `07-capture/<id>/output/`. They must not be written in `06-build/`.

Citations:
- DS-4 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\06-build\CONTEXT.md:21-22` — "Renders go to `../07-capture/<id>/output/`. Do not write MP4s here."
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:15-16` — "`<id>/output/` holds the runs."

## Q3
What is the difference between a check / stills / strip, a preview, and a render (master)?

- Check / stills / strip: scene-scope checks in build. A check is not a master.
- Preview: a review copy to watch. No approval needed.
- Render (master): the master plus QA. Needs a current plan approval.

Citations:
- DS-4 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\06-build\CONTEXT.md:13` — "Check with `npm run check`, `stills`, and `strip`."
- DS-4 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\06-build\CONTEXT.md:19` — "A check is not a master."
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:13` — "`npm run preview -- <id>` to watch a copy. `npm run render -- <id>` for the master. It needs a current plan approval."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:21-22` — "`check/stills/strip/audio` — scene-scope checks" ; "`preview` (review render, no approval needed) vs `render` (master + QA, needs current plan approval)."

## Q4
When is a current plan approval required before a render?

A current plan approval is required before `npm run render -- <id>` for the master. Preview does not need approval.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:13` — "`npm run render -- <id>` for the master. It needs a current plan approval."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:22` — "`preview` (review render, no approval needed) vs `render` (master + QA, needs current plan approval)."

## Q5
What must be shown at Stop 1, and how is plan approval recorded?

At Stop 1 show premise, key moments, look, the board, and deliberate exceptions. End the turn. Record the owner's words with:

`npm run approve -- <id> --stage plan --note "<their words>"`

Citations:
- DS-2 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\03-design\CONTEXT.md:21-24` — "Stop 1. Show premise, key moments, look, the board, and deliberate exceptions. End the turn. Record the owner's words:" plus the approve command for `--stage plan` with `--note "<their words>"`.
- DS-1 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\CONTEXT.md:15` — "Stop 1 is this stage's [03-design] approval" — supporting location context.

## Q6
What must be shown at Stop 2, and how is release approval recorded?

At Stop 2 show the master and `review.md`. End the turn. Then record with:

`npm run approve -- <id> --stage release --note "<their words>"`

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:21-24` — "Stop 2. Show the master and `review.md`. End the turn. Then:" plus the approve command for `--stage release` with `--note "<their words>"`.
- DS-1 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\CONTEXT.md:19` — "Stop 2 is this stage's [07-capture] approval" — supporting location context.

## Q7
When does Stop 1 become stale and require re-approval?

Stop 1 becomes stale and requires re-approval when a change edits the approved brief, references, or design. A repair also requires re-approval because repair withdraws approvals.

Citations:
- DS-3 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\04-shot-plan\CONTEXT.md:22` — "If a change edits the approved brief, references, or design, Stop 1 is stale. Ask again."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:23` — "`repair --note` — approvals bound to input/video hashes; repair withdraws both." — supporting repair route to re-approval.

## Q8
What does `repair` do to existing plan and release approvals?

`repair` withdraws both plan and release approvals.

Citations:
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:23` — "`approve --stage plan|release` / `repair --note` — approvals bound to input/video hashes; repair withdraws both."
- DS-8 — `C:\Users\A-Med\Desktop\animation-studio\package.json:24` — `"repair": "node workflows/studio/cli/tools/studio.mjs repair"` — verb exists as CLI command.

## Q9
Where do approvals live, and what keeps them current?

Approvals live in `projects/<id>/production.json`, written by the CLI, not in a stage file. They are current only while the stored render video/input hashes match.

Citations:
- DS-7 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\projects\CONTEXT.md:12-13` — "`production.json` is written by the CLI. Approvals live there, not in a stage file."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:29` — "Film state: `../projects/<id>/production.json` (render video/input hashes; approvals current only while matching)."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:23` — "approvals bound to input/video hashes" — supporting currency condition.
- DS-7 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\projects\CONTEXT.md:4` — "Pointers only." — the film log holds pointers, not the work.

## Q10
What files constitute a complete capture delivery for one run?

A complete capture delivery for one run is `<id>/output/` holding the runs, with `<id>/review.md`, `playback-review.json`, and `build-log.md` beside it, with each video SHA-256 recorded in `review.md` and `playback-review.json`.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:15-16` — "`<id>/output/` holds the runs. `<id>/review.md`, `playback-review.json`, and `build-log.md` sit beside it."
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:13` — "Fill `<id>/playback-review.json` and `<id>/review.md`: what was watched and heard, reference-bar results, board reconciliation, staging against the master, exceptions, unverified items, and each video SHA-256."

## Q11
What playback check is required for each delivered video?

Watch each delivered video continuously and listen, or document intentional silence. Stills and QA are not that viewing.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:13` — "Watch each delivered video continuously and listen, or document intentional silence. Stills and QA are not that viewing."

## Q12
What is the completion condition for 07-capture?

All of: a current master, no QA failures, a complete playback record for that run, and a `review.md` with no `TODO` that names each SHA-256. File presence is not acceptance.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:19` — "A current master, no QA failures, a complete playback record for that run, and a `review.md` with no `TODO` that names each SHA-256. File presence is not acceptance."

## Q13
What is the relationship between QA status and creative acceptance?

Machine QA, file presence, stills, and preview are not creative acceptance. Missing evidence never passes. Tools do not approve films; plan/release approvals are owner decisions.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:13` — "Stills and QA are not that viewing."
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:19` — "File presence is not acceptance."
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:28-29` — "Do not treat QA as acceptance. An interrupted run with no finish record stays pending."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:37` — "Tools do not approve films. Plan/release approvals are owner decisions recorded via `approve` (or agent on explicit chat "approved" + `--note "<their words>"`). Machine QA statuses (PASS/FAIL/WARN/NOT APPLICABLE/NOT TESTED) are not creative acceptance; missing evidence never passes."

## Q14
What is the studio's publish rule?

The workspace never publishes. Do not publish/upload.

Citations:
- DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:26` — "The workspace never publishes."
- DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:40` — "Do not publish/upload; do not edit outside workspace."

## Q15
What is the correct response if asked for a broadcast specification, resolution / frame rate, version-number scheme, colour-management rule, safe-area rule, or social-cutdown spec?

“Unavailable from the supplied delivery-standards source.”

Missing spec types not in DS-1–DS-8: broadcast specification, resolution / frame rate spec, version-number scheme, colour-management rule, safe-area rule, social-cutdown spec.

Citations:
- Coverage route — `02-folder-preparation/output/motion-delivery-folder/coverage-map.md:24` — Q15 explicit unavailability, none in DS-1–DS-8.
- Answer route — `02-folder-preparation/output/motion-delivery-folder/answer-rules.md:6,13` — if map says explicit unavailability answer exactly that sentence; MP4 is the only format claim; no resolution, frame rate, codec, colour, naming-pattern, version-number, or broadcast claims exist.
- Source scope verified in DS-1 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\CONTEXT.md:4`; DS-2 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\03-design\CONTEXT.md:21-24`; DS-3 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\04-shot-plan\CONTEXT.md:18-22`; DS-4 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\06-build\CONTEXT.md:15-22`; DS-5 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\07-capture\CONTEXT.md:12-29`; DS-6 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\cli\tools\CONTEXT.md:22-40`; DS-7 — `C:\Users\A-Med\Desktop\animation-studio\workflows\studio\projects\CONTEXT.md:10-14`; DS-8 — `C:\Users\A-Med\Desktop\animation-studio\package.json:13-24` — none states the requested specs.
