# OpenGorky

This repo lives in `/srv/git` — the only git-synced tree on this server (mirrors GitHub).
Server conventions: see `/srv/CLAUDE.md`.

- Declare deploy targets in `.deploy.yml` (schema: `/srv/_ops/deploy.schema.md`).
- Served output → `/srv/<entity>/www/<path>`; data → `/srv/<entity>/data` (never web-served).
- Deploy: `deploy OpenGorky [--to <entity>:/path]`   ·   Sync: `sync OpenGorky` (or `sync --all`).
