# Chess guide — image checklist

Drop your screenshots in this folder using these exact filenames so `index.html` picks them up automatically.

**Capture tips:** **Shift+F3** = lossless PNG crop of the top open UI panel (Quick2DChessBoard when Tab overlay is open). **Print Screen** = full-screen JPG. See the guide appendix for F3 SnapShotCam.

---

## Required (core guide figures)

| File | What to capture |
|------|-----------------|
| `01-south-parthenon-game.jpg` | Wide shot: South Parthenon exterior with the **3D board** and an **active game** (pieces on board, player cage visible if possible). |
| `02-ministele-front.jpg` | **Chess-Stele front** trigger: Level, Piece Labels, Style, Predict, Puzzles, Custom, START/Play/Playing, red Clear, status lines, and **Leorik sliders** (Easy+). |
| `03-ministele-back-history.jpg` | **Back** panel in **History** mode: header "History", numbered move list, mini 2D board. |
| `04-ministele-back-puzzles.jpg` | **Back** panel with **Puzzles** selected on front: puzzle list rows, green/orange row colors if possible. |
| `05-ministele-back-custom.jpg` | **Back** panel in **Custom** edit: palettes, empty or partial board, FEN field, Clear Board / Play controls. |

PNG or WebP also work — update the `src` paths in `index.html` if you use different extensions.

---

## Strongly suggested (helps new players)

| File | What to capture |
|------|-----------------|
| `06-3d-board-selection.jpg` | First-person view: **white piece selected**, green legal-move highlights on the outdoor board (either style). |
| `07-practice-landing-ring.jpg` | **Practice (level 0)**: melee + zoom aim showing the **orange landing ring** on a square. |
| `18-standard-selection.jpg` | **Style: Standard** — same selected piece/legal squares; show **flat blue + green circles only** (no runic auras). Match pose to `19` if possible. |
| `19-wizard-selection.jpg` | **Style: Wizard** + **Predict: On** — same position as `18`; runic **piece** aura plus full tactical hint set. Compare **Predict Off** to `23`. |
| `08-wizard-capture.jpg` | **Wizard** style: mid-slide or capture smoke + hit light on the 3D board. |
| `09-puzzle-solved.jpg` | HUD/status showing **`PUZZLE n SOLVED!`** or standing on Black King to advance. |
| `24-puzzle-wrong-x.jpg` | **Puzzle coach:** **Predict: Hint** + active puzzle — ❌ (`puzzle_hint_x` / `<sprite=1920>`) on a wrong square while aiming (2D or 3D). Optional; pair with 🟢 `greenChessCircle` / `<sprite=783>` on the mate square. |
| `10-status-three-lines.jpg` | Chess-Stele/main **idle** status crop (3 lines): e.g. `Chess 1 - Easy` / turn / `Position: D3`. |
| `11-tactical-caution.jpg` | **Caution overlays:** **red** immediate attackers + **yellow** move-target defenders + optional **blue-tinted white backup pieces** on an **orange** target on a **2D board** (Chess2DUI dots + 💥/⚠️ corner badges). Requires **Predict: On** or Hint and **Piece Labels ≠ None**. Optional matching ⚠️/💥 on 3D labels. |
| `12-black-scout-hold.jpg` | **Passive scout:** crosshair held on a black pawn/knight ~1 s — small **red diamonds** on empty move squares, **large red diamonds** under threatened white pieces (**Predict: On** or Hint). Wizard + Predict On: red auras on 3D instead. |
| `17-white-inspect-hold.jpg` | **Friendly inspect:** crosshair held on another white piece ~1 s — small **blue diamonds** on empty move squares, **large blue diamonds** above threatened black pieces (**Predict: On** or Hint). Wizard + Predict On: blue auras on 3D instead. White-base diamond PNGs are tinted blue in-engine. |
| `16-quick2d-chess-tab-board.png` | **Full Tab overlay:** board + **3-line status** + move log. Press **H** to cycle **Predict: Off → On → Hint → On + Hint** (label on **3DGameMessageText**). Easiest: **Shift+F3** while panel is open. |

---

## New — status & 2D overlay art (2026 UI update)

These document the **compact Tab status**, **Chess-Stele pending-move status**, and overlay glyphs.

| File | What to capture | Priority |
|------|-----------------|----------|
| `20-tab-status-compact.png` | **Tab board only** — tight crop of the **3-line status** during a puzzle: `Puzzles 1/39 - Easy` / `Selected: Queen` / `Position: D3 (Move to H7?)`. Shift+F3 while Tab overlay is open. | **High** |
| `21-stele-status-pending.jpg` | **Chess-Stele or main UI** — status crop showing **four lines** with pending move: header / `Selected: …` / `Move to H7?` / `Position: …` | **High** |
| `22-2d-overlay-glyphs.png` | **Close-up** of a 2D board cell area showing Chess2DUI sprites with matching emoji from `HelperDocs/GameSpriteTags.txt`: 🟢 `greenChessDot` (`<sprite=783>`), 🟠 `orangeChessCircle` (`<sprite=659>`), 🟣 `purpleChessDot` (`<sprite=845>`), ♦️ `chessDiamond` / `chessDiamondLarge` (white base; tinted red for scout `<sprite=3282>` or blue for inspect `<sprite=3068>` on 3D labels), 💥/⚠️ badges (`<sprite=1330>` / `<sprite=307>`), and optional **blue-tinted white backup pieces** on an orange target. Capture with **Predict: On** or Hint and **Piece Labels ≠ None**. Puzzle coach 🟢 circle + ❌ X → capture separately as `24-puzzle-wrong-x.jpg`. | **Medium** |

**Tab status setup:** Start a puzzle, stand on a white piece with a legal move, RMB a destination so `(Move to …?)` appears on line 3.

**Chess-Stele status setup:** Same game state but crop the Chess-Stele status text (four separate lines, not combined).

**Blue backup setup:** With **Predict: On** or Hint, select a white piece and hover or RMB an **orange** legal destination where at least one **other** white piece attacks that square (e.g. queen to d6 with a rook on d1). Capture **blue-tinted white pieces** on 2D for `11` or `22`.

---

## Piece vs Piece Practice (Custom mode — beginner drill)

Unique to **South Parthenon Custom mode**. Capture the mini board **after Play** (or during edit) showing only two pieces — one White, one Black, same type. Include the **7-second center banner** when possible (e.g. *King Practice 50 Moves*).

| File | What to capture |
|------|-----------------|
| `13-piece-practice-king-vs-king.jpg` | **King vs King** — two kings on the Custom mini board (and/or 3D board); banner visible if timing allows. |
| `14-piece-practice-pawn-vs-pawn.jpg` | **Pawn vs Pawn** — mirrored pawns on the edit/play board. |
| `15-piece-practice-knight-vs-knight.jpg` | **Knight vs Knight** — mirrored knights; optional: legal L-move hints during play. |

---

## Optional extras

| File | What to capture |
|------|-----------------|
| `23-wizard-predict-off.jpg` | **Wizard + Predict Off** — green orbs (legal moves), blue orb (standing), orange aura on RMB destination; no purple or white-piece runic aura. |
| `24-tab-overlay-normal-mode.png` | Tab board after **H** → **Predict: Off** — green dots + blue standing circle only (no yellow/red/purple). |

---

## Tips for consistent screenshots

- Use the same time of day / lighting if possible.
- Hide debug overlays and console unless documenting them.
- **Shift+F3** saves lossless PNG crops of open UI panels to this folder (or `Escaper/SnapShots/` fallback).
- **Print Screen** saves full main-camera JPG; **F3** opens SnapShotCam for fly doc shots.
- 1920×1080 or 1600×900 JPEG at ~85% quality is fine for web photos; use PNG for UI panel crops and status text.
- Crop Chess-Stele shots so button labels are readable.
- Chess2DUI sprites include baked black shadows — capture at 100% scale; avoid heavy JPEG on small UI crops.
