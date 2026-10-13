# 03 Design

## PURPOSE
Decide the film's look, structure, and draft board. Stop 1 happens here.

## ENTER_WHEN
Status says `3 Design` or `Stop 1`.

## INPUTS
`../01-brief/<id>/brief.md` and `../02-references/<id>/references.md`. Sheets of any reference used for a visual decision. Read only the guide this idea needs: `story.md`, `design.md`, `acting-continuity.md`, `stylized-3d.md`, or one file in `examples/`.

## PROCESS
Write the premise and beats. For each borrowed mechanism, say what changes and what is left out. Set composition, palette, type, material, light, depth, camera, movement, holds, and sound. Renderer is React by default, or a Canvas2D comp. Add Three.js inside a scene only when a shot needs it. Write 5–7 checks you can see in frames or playback. Draft `<id>/storyboard.md` from `template/storyboard.md` (detail only, not any prior film's story). Include a staging table: volume, camera/depth, action, motion. A plan table is a prediction, not evidence.

## OUTPUTS
`<id>/design.md` and draft `<id>/storyboard.md`.

## COMPLETION
Both exist and contain no `TODO`. The draft covers the whole film.

## HUMAN_REVIEW
Stop 1. Show premise, key moments, look, the board, and deliberate exceptions. End the turn. Record the owner's words:

`npm run approve -- <id> --stage plan --note "<their words>"`

## BOUNDARIES
Do not build. Do not open `../06-build/engine.md`.
