# 07 Capture

## PURPOSE
Render, watch, and review the film. This is the last stage. Stop 2 happens here.

## ENTER_WHEN
Status says `7 Capture` or `Stop 2`.

## INPUTS
The build in `../06-build/<id>/`. `cognition.md` only if you are checking how a review was reasoned.

## PROCESS
`npm run preview -- <id>` to watch a copy. `npm run render -- <id>` for the master. It needs a current plan approval. Watch each delivered video continuously and listen, or document intentional silence. Stills and QA are not that viewing. Fill `<id>/playback-review.json` and `<id>/review.md`: what was watched and heard, reference-bar results, board reconciliation, staging against the master, exceptions, unverified items, and each video SHA-256.

## OUTPUTS
`<id>/output/` holds the runs. `<id>/review.md`, `playback-review.json`, and `build-log.md` sit beside it. `tools/` runs render and QA.

## COMPLETION
A current master, no QA failures, a complete playback record for that run, and a `review.md` with no `TODO` that names each SHA-256. File presence is not acceptance.

## HUMAN_REVIEW
Stop 2. Show the master and `review.md`. End the turn. Then:

`npm run approve -- <id> --stage release --note "<their words>"`

The workspace never publishes.

## BOUNDARIES
Do not treat QA as acceptance. An interrupted run with no finish record stays pending.
