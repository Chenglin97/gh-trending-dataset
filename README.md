# GitHub events dataset — August 2026

Real GitHub Archive events for ~500 popular open-source repositories,
August 2026. This is the dataset for a take-home engineering task.

**Download**: see the [latest release](../../releases/latest) for the data
file.

## Format

- Gzipped JSON Lines (`.jsonl.gz`) — one JSON object per line, each line a
  single GitHub event (the same shape GH Archive and GitHub's webhook
  payloads use: `id`, `type`, `actor`, `repo`, `payload`, `created_at`).
- **Size**: 67MB compressed.
- **Events**: ~137K.
- **Repos**: ~500 popular, active, real open-source projects.
- **Order**: one event per line, in the order they arrived — as with any
  real webhook feed, that's mostly but not strictly chronological.

To preview a sample event:

```
gunzip -c github-events-2026-08-top500repos.jsonl.gz | head -1
```
