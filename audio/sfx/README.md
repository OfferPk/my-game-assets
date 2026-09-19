# audio/sfx

One-shot sound effects (shots, hits, UI clicks, pickups).

## Conventions

- Format: prefer `.mp3` or `.ogg` for runtime; keep sources elsewhere if needed.
- Naming: `action-or-object.ext` (e.g. `shoot.mp3`, `hit-enemy.ogg`).
- Keep clips short and normalized in loudness when possible.

## Pending move

Root file `shoot.wav.mp3` belongs here as `shoot.mp3`. Relocate with a local `git mv` when convenient so git history for the blob is preserved.
