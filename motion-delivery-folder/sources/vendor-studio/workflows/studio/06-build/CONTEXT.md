# 06 Build

## PURPOSE
Draw the film in code. The renderer lives here.

## ENTER_WHEN
Status says `6 Build`.

## INPUTS
`../04-shot-plan/<id>/shots.md` and `storyboard.md`. Plates in `../05-plates/media/<id>/`. Read `engine.md`, then only the engine files this film needs. `colour-compositing.md` only if the shot composites. `../04-shot-plan/audio.md` only when building cues.

## PROCESS
Work in `<id>/src/` or `<id>/film.js`. Passes: layout, key poses, rough motion, polish, light, effects, sound. Every frame is a pure function of frame number and declared inputs. Characters on twos, camera and particles on ones, unless the brief says otherwise. No CSS animations or `backdrop-filter`. Implement each shot's temporal idea from `../04-shot-plan/dynamic-shots.md`; audit for slideshow (still-swap, purposeless zoom) before check. After a cue change, `npm run audio -- <id>`. Check with `npm run check`, `stills`, and `strip`. Scene code is timing authority once build starts. Reconcile the board. Do not drop a planned action quietly.

## OUTPUTS
`<id>/` code and `project.json`. `engine/` is the renderer. `assets/` holds fonts and shared build assets. `tools/` runs check, stills, strip, and audio.

## COMPLETION
The scene code matches the board well enough to capture. A check is not a master.

## BOUNDARIES
Renders go to `../07-capture/<id>/output/`. Do not write MP4s here.
