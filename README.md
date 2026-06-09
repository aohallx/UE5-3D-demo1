# UE5 Zombie Japan

Third-person action prototype built in **Unreal Engine 5.4** with melee and ranged combat, stealth takedowns, equipment management, and AI-driven enemies in a Japanese-inspired environment.

> Portfolio showcase repo. Source project lives locally; this repository contains screenshots, demo video, feature notes, and architecture documentation for portfolio and public viewing.

![Editor overview](media/screenshots/01-editor-overview.png)

## Quick links

| Resource | Location |
|----------|----------|
| Feature list | [docs/FEATURES.md](docs/FEATURES.md) |
| Architecture notes | [docs/ARCHITECTURE.md](docs/ARCHITECTURE.md) |
| Screenshots | [media/screenshots/](media/screenshots/) |
| Demo video | [media/video/](media/video/) |

## Highlights

- **Camera** — button toggle between third-person and first-person (`IA_PerspectiveChange`)
- **Combat** — sword melee with animation notifies, dodge roll, hit reactions, and camera shake feedback
- **Ranged weapons** — pistol, AK, sniper (with scope UI), bow, and throwable objects
- **Stealth** — paired assassination animations with on-screen prompt UI
- **Equipment** — slot-based weapon system with data tables and in-game equipment menu
- **AI** — behavior trees for patrol, chase, investigate, and attack; separate boss AI controller
- **World** — Japanese shrine Megascans assets, landscape tooling, Ultra Dynamic Sky

## Tech stack

| | |
|---|---|
| Engine | Unreal Engine 5.4 |
| Language | Blueprints (visual scripting) |
| Input | Enhanced Input (`IMC_Default`) |
| AI | Behavior Trees, Blackboards, EQS-style patrol tasks |
| Rendering | DX12 / SM6, Virtual Shadow Maps, Virtual Textures |
| Plugins | Motion Warping, Landmass, Landscape Patch, Modeling Tools |

## Controls (default)

| Action | Input |
|--------|-------|
| Move / Look | WASD + Mouse |
| Jump | Space |
| Sprint | Shift |
| Crouch | Ctrl |
| Attack | LMB |
| Dodge | (bound in `IA_Dodge`) |
| Interact / Assassinate | (bound in `IA_Interact` / `IA_Assasin`) |
| Equipment menu | (bound in `IA_EquipmentMenu`) |
| Target lock | (bound in `IA_TargetLock`) |
| Sniper aim | (bound in `IA_Snipe_Aim`) |
| Vault | (bound in `IA_Vault`) |
| Toggle 1st / 3rd person | (bound in `IA_PerspectiveChange`) |

## Demo video

Add a gameplay capture to `media/video/demo.mp4`, then embed it here:

```markdown
[![Gameplay demo](media/screenshots/02-gameplay-thumb.png)](media/video/demo.mp4)
```

**Suggested capture checklist**
- 30–90 seconds of combat (melee + ranged)
- One stealth assassination
- Enemy AI chase or patrol moment
- Equipment swap
- One environment shot (shrine / landscape)

## Screenshots

| | |
|---|---|
| Editor / project overview | `01-editor-overview.png` |
| Combat | `02-combat.png` *(add)* |
| Stealth assassination | `03-stealth.png` *(add)* |
| Equipment UI | `04-equipment.png` *(add)* |
| AI / enemies | `05-enemies.png` *(add)* |
| Environment | `06-environment.png` *(add)* |

See [media/screenshots/README.md](media/screenshots/README.md) for capture tips.

## Project structure (source)

Local Unreal project path:

```
C:\Users\aohal\OneDrive\Documents\Unreal Projects\japan1
```

Key content folders:

```
Content/
├── ThirdPerson/          # Player character, input, maps (Main, ThirdPersonMap)
├── Blueprints/           # Attack system, player stats, enemy spawner, anim notifies
├── Equipment_System/     # Weapons, slots, equipment UI
├── AI/                   # Regular + boss behavior trees and controllers
├── Characters/RPG_Character/  # Locomotion, combat, stealth animations
├── 3dAssets/Weapons/     # Sword, bow, pistol, AK, sniper, shield
├── UI/                   # HUD, boss bar, sniper scope, prompts
├── Audio/                # Footsteps, gunshots, sword hits, grunts
├── FXs/                  # Combat and environment VFX
└── Megascans/            # Japanese environment surfaces and props
```

## Portfolio usage

This repo is designed to link from a portfolio site. Suggested embed pattern:

- **Hero** — best environment or combat screenshot
- **Video** — `media/video/demo.mp4` or YouTube/Vimeo link
- **Details** — link to [FEATURES.md](docs/FEATURES.md) and [ARCHITECTURE.md](docs/ARCHITECTURE.md)
- **Tech tags** — `Unreal Engine 5`, `Blueprints`, `Behavior Trees`, `Enhanced Input`, `Motion Warping`

## Local development

1. Open `japan1.uproject` in Unreal Engine 5.4
2. Default map: `Content/ThirdPerson/Maps/ThirdPersonMap`
3. Play-in-editor to test combat, AI, and equipment flows

> **Note:** The full `.uasset` project is not committed here (binary size + marketplace assets). This repository is documentation and media only.

## Author

**Aidan O'Halloran** — [GitHub](https://github.com/aohallx)

## License

Portfolio showcase only. Game assets may include third-party marketplace content (Megascans, Paragon, Fab, etc.). Not licensed for redistribution.
