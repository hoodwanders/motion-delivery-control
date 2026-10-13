# Studio

## PURPOSE
The animation workflow. Code-drawn films, captured to MP4.

## ENTER_WHEN
The task is to make, continue, or repair a film.

## PROCESS
Run `npm run status -- <id>`. Enter only the stage it names. The log at `projects/<id>/CONTEXT.md` points at that film's files. It does not hold them.

## CHILD_WORKSPACES
- `01-brief/` — what the film is, before any look is chosen
- `02-references/` — technique records, then the film's reference notes
- `03-design/` — look, story, and the draft board. Stop 1 is this stage's approval
- `04-shot-plan/` — frame ranges, cues, and the final board
- `05-plates/` — this film's supplied and generated images. Not reference footage
- `06-build/` — scene code and the renderer
- `07-capture/` — renders, playback, and release review. Stop 2 is this stage's approval
- `projects/` — log only
- `cli/` — status, approve, repair

## BOUNDARIES
Career, research, and experiments are other workflows. Do not load them for a film.
