# log-socialpredict-tasks

Archive repo for task and agent logs that are migrated out of SocialPredict repositories such as `socialpredict` and `socialpredict-auto`.

## Convention

Canonical current snapshots live under:

`current/<source-repo>/<ref-kind>/<ref-name>/<source-commit>/`

Legacy or non-canonical snapshots live under:

`archives/<source-repo>/<ref-kind>/<ref-name>/<source-commit>/`

Each snapshot contains:

- `manifest.json`: source metadata, migration metadata, and the migrated log roots.
- `files/`: an exact mirror of the original source-repo paths for the archived files.
- `SHA256SUMS`: checksum inventory for larger snapshots.

Ref names are mirrored directly into the path. A branch like `fix/checkpoint20251020-80` becomes nested path components under `branches/`.

This keeps the source tree intact while allowing multiple snapshots from branches, tags, or direct commits to coexist.

Examples:

- `current/socialpredict-auto/branches/fix/checkpoint20251020-80/<commit>/files/.codex-reports/...`
- `archives/socialpredict/branches/main/<commit>/files/README/CHECKPOINTS/...`
- `archives/socialpredict/tags/<tag>/<commit>/files/codex-reports/...`

## Current snapshot

The primary current snapshot in this repo is `.codex-reports` from `socialpredict-auto` branch `fix/checkpoint20251020-80` at commit `eaf570e1348b8c174f85e20de6d292302f1c0953`.

It is stored at `current/socialpredict-auto/branches/fix/checkpoint20251020-80/eaf570e1348b8c174f85e20de6d292302f1c0953/`.

## Legacy archive

The earlier `socialpredict` checkpoint migration remains archived under `archives/socialpredict/branches/main/662fa812646d7da7c04c8af794f17d41621bef36/`.

At migration time on 2026-04-10, no `codex-reports` directory was present in the local `socialpredict` working tree or in `origin/main`.
