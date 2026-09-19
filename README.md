# my-game-assets

Shared game asset library for OfferPk projects.

## Status

Small, early collection. One sound effect lives at the repo root; folders below are the **intended** layout for new assets.

## How to use these assets

1. Prefer referencing paths under the folders documented here once files are moved into them.
2. Until then, the only playable asset is the root shoot SFX (see inventory).
3. Import or copy assets into your game project (Unity, Godot, web, etc.) — this repo does not ship a runtime.
4. Keep filenames lowercase kebab-case or snake_case; one extension only (e.g. `shoot.mp3`, not `shoot.wav.mp3`).

### Example (conceptual)

```text
# After relocating the SFX into audio/sfx/:
audio/sfx/shoot.mp3  →  play on player fire / weapon trigger
```

Consumers should treat paths as stable once assets sit under `audio/` or `images/`.

## Current inventory

| Path | Type | Notes |
|------|------|--------|
| `shoot.wav.mp3` | Audio (MP3) | Shoot / fire SFX. Double extension is historical; treat as MP3. **Intended home:** `audio/sfx/shoot.mp3` (not moved in this cleanup — binary relocate needs a local `git mv`). |

## Intended layout

```text
.
├── README.md
├── .gitignore
├── shoot.wav.mp3          # legacy location (see inventory)
├── audio/
│   ├── sfx/               # one-shot sound effects
│   └── music/             # loops / BGM
└── images/
    ├── sprites/           # characters, tiles, VFX frames
    └── ui/                # HUD, buttons, icons
```

Each folder has a short README describing what belongs there.

## Adding assets

- Put new SFX in `audio/sfx/`, music in `audio/music/`.
- Put sprites in `images/sprites/`, UI art in `images/ui/`.
- Update this inventory table when you add or move files.
- Do not commit huge uncompressed work files, secrets, or personal exports.

## License / attribution

Not specified. Confirm rights before redistributing assets in a shipped game.
