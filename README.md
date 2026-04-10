# log-socialpredict-tasks

Archive repo for task and agent logs that are migrated out of `socialpredict`.

## Convention

Each archived snapshot lives under:

`archives/<source-repo>/<ref-kind>/<ref-name>/<source-commit>/`

Each snapshot contains:

- `manifest.json`: source metadata, migration metadata, and the migrated log roots.
- `files/`: an exact mirror of the original source-repo paths for the archived files.

This keeps the source tree intact while allowing multiple archives from branches, tags, or direct commits to coexist.

Examples:

- `archives/socialpredict/branches/main/<commit>/files/README/CHECKPOINTS/...`
- `archives/socialpredict/tags/<tag>/<commit>/files/codex-reports/...`

## Current archive

The first snapshot in this repo archives `README/CHECKPOINTS` from `socialpredict` branch `main` at commit `662fa812646d7da7c04c8af794f17d41621bef36`.

At migration time on 2026-04-10, no `codex-reports` directory was present in the local `socialpredict` working tree or in `origin/main`.
