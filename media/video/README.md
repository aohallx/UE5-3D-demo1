# Demo video

Add a short gameplay reel for portfolio visitors.

## Recommended file

| File | Format | Length |
|------|--------|--------|
| `demo.mp4` | H.264 MP4 | 30–90 seconds |

## What to show

1. Establishing shot of the Japan environment
2. Sword combat + hit feedback
3. Ranged weapon (pistol or sniper)
4. Stealth assassination
5. Enemy AI reacting (chase or attack)
6. Quick equipment menu swap

## Recording options

### In-editor (quick)

1. **PIE** → Windows **Win+G** Game Bar, or OBS Studio
2. Record at 1080p / 60fps
3. Trim in DaVinci Resolve, Clipchamp, or similar

### Sequencer (polished)

1. Create a Level Sequence with camera cuts
2. Use **Movie Render Queue** for clean output without UI
3. Export MP4 and place here as `demo.mp4`

### YouTube / Vimeo (optional)

If the file is large, upload externally and link from the root `README.md`:

```markdown
**[Watch gameplay demo on YouTube](https://youtu.be/YOUR_ID)**
```

Keep a local `demo.mp4` only if size is reasonable for GitHub (prefer &lt; 25 MB, or use Git LFS).

## Git LFS (optional)

For videos over ~25 MB:

```bash
git lfs install
git lfs track "*.mp4"
git add .gitattributes
```
