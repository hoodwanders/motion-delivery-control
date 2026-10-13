# 04 Shot plan

## PURPOSE
Turn the approved design into shots, a final board, and asset prompts.

## ENTER_WHEN
Status says `4 Shot plan`. Plan approval must be current.

## INPUTS
`../03-design/<id>/design.md` and its draft board. `audio.md` only if the film has sound. `../03-design/acting-continuity.md` only if a character acts or shots connect.

## PROCESS
For each shot: purpose, integer range `[start, end)`, action, camera, layers, effects, transition, sound cues, continuity. Every shot must have a temporal idea: camera change, subject action, env motion, parallax, lighting progression, or a justified still hold. A still image is compositable material, never a static slide by default. See `dynamic-shots.md` only when a shot risks slideshow. Finalize `<id>/storyboard.md` here. Reconcile ranges, contacts, cues, and assets with the board. Mark every asset code-drawn, supplied with a path, or a generated image. A generated image is a fenced prompt. Wait for the file or for "use placeholders." Received images go to `../05-plates/`, not here.

## OUTPUTS
`<id>/shots.md` and `<id>/storyboard.md`.

## COMPLETION
Both exist, contain no `TODO`, and agree. Do not build without the board.

## BOUNDARIES
If a change edits the approved brief, references, or design, Stop 1 is stale. Ask again.
