# AGENTS.md

Rules to hand an AI agent before it edits a repo. Copy this file in and it stops guessing. Short on purpose.

## Stack

- TypeScript for anything web. Bun, not npm. Vite + React for apps.
- Go or Rust for CLIs. Podman, never Docker. systemd for services on Linux.
- SQLite for small local state; Postgres when it is shared.

## Code

- Smallest change that fully solves the task. Delete before adding.
- No speculative abstractions, no unused config, no "for later" code.
- Never cut: validation, error handling, security, accessibility.
- Tests for anything with a branch, and run them before saying done.

## UI

- No AI slop: no purple gradients, no emoji as icons, no centred hero over three feature cards.
- One typeface family, two at most. One accent colour. A real spacing scale.
- Motion: one authored moment, and respect `prefers-reduced-motion`.

## Repo hygiene

- Conventional commits. No secrets in the tree — `.env` stays out.
- Do not reformat files you did not touch.
- Update the README when behaviour changes.

## When unsure

Say so, name the missing fact, then check the source or the docs. Do not guess.
