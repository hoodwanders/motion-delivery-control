# Tools — CLI and pipeline tools

## PURPOSE
FACTORY: `studio.mjs` CLI plus film, render, QA, soundtrack, and reference tools. Gates live in `../pipeline/`. Tools write `output/` and `production.json`.

## ENTER_WHEN
Running any `npm run` film command, or maintaining CLI/tool scripts.

## INPUTS
- Film id + stage/variant flags (`--scope`, `--spec <variant>` for `project.<variant>.json`).
- Film spec: `../projects/<id>/project.json`; scenes/cues for audio/QA tools.

## REFERENCES
- Pipeline steps: `../pipeline/CONTEXT.md`. Open only the step being changed.
- Engine records: `../knowledge/engine.md` ("What a render records", QA statuses, sound) and `../engine/CONTEXT.md` for renderer behavior.
- Tests: `../tests/` via `npm test`.

## PROCESS
Use `npm run` commands; `studio.mjs` picks the right tool from the spec:
- `new/status/refs/studio` — scaffold, state/routing, reference intake/search, browser preview + board.
- `check/stills/strip/audio` — scene-scope checks; `--spec <variant>` picks variant spec.
- `preview` (review render, no approval needed) vs `render` (master + QA, needs current plan approval).
- `approve --stage plan|release` / `repair --note` — approvals bound to input/video hashes; repair withdraws both.
- `experiment`, `experiment:audio`, `experiment:fixtures` — isolated trials into `../output/experiments/` only; never write film production records.
- Python tools (`qa.py`, `soundtrack.py`, `watch_refs.py`, etc.) run offline prep/measurement; scenes validate via `prepare()`/zod.

## OUTPUTS (where they go)
- Film renders/QA/logs: `../output/<id>/<run>/` + `evidence/<format>/` (`manifest.json`, `frames.json`, `checkpoints/`, `qa/`), console logs + exit codes retained in run dir.
- Film state: `../projects/<id>/production.json` (render video/input hashes; approvals current only while matching).
- Reference index: `../references/index.json` (via `refs`).
- Audio builds from scene cues (`audio` / `soundtrack.py`); voice/music/sfx per spec `soundtrack` block, silent if absent.

## COMPLETION
Command exits 0 with expected artefacts in the run dir / state file. `npm test` passes after any tool/engine change. An interrupted run with no finish record stays pending investigation — never infer success from partial files.

## HUMAN_REVIEW
Tools do not approve films. Plan/release approvals are owner decisions recorded via `approve` (or agent on explicit chat "approved" + `--note "<their words>"`). Machine QA statuses (PASS/FAIL/WARN/NOT APPLICABLE/NOT TESTED) are not creative acceptance; missing evidence never passes.

## BOUNDARIES
Not here: renderer implementations (`../engine/CONTEXT.md`), reference content (`../references/CONTEXT.md`), film docs/scenes (`../projects/CONTEXT.md`), craft guidance (`../knowledge/CONTEXT.md`). Do not publish/upload; do not edit outside workspace.

## CHILD_WORKSPACES
- `studio.mjs` — CLI entry; start here for command behavior.
- `film.mjs`, `render.mjs`, `sheet.mjs`, `serve.mjs` — film/render/sheet/preview paths.
- `qa.py`, `qa_marks.py`, `pop_scan.py`, `soundtrack.py`, `audio_audit.py`, `audio-audit.mjs`, `playback-review.mjs`, `refs.py`, `watch_refs.py`, `experiment.mjs`, `experiment_report.py` — specialised tools; open only the one the task needs.
- No per-film state lives here.
