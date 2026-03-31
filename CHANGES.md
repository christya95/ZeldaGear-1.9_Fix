# 🔄 ZeldaGear 1.9 – Fix Overview

This file summarizes the main data/JSON changes between the **original ZeldaGear 1.9** jar and this **fixed** version.

> Note: The original `OLD_ZeldaGear-1.9.jar` is not included in this repo, so this is a **behavior + file-level** summary, not an auto-generated line-by-line diff.

## 🪝 Hookshot / Longshot fixes

**Files changed**
- `mods/ZeldaGear-1.9/Server/Item/Items/Tools/Hookshot.json`
- `mods/ZeldaGear-1.9/Server/Item/Items/Tools/Longshot.json`
- `mods/ZeldaGear-1.9/Server/Item/RootInteractions/Tools/Root_Hookshot_Primary.json`
- `mods/ZeldaGear-1.9/Server/Item/Interactions/Tools/Zelda_Hookshot_Primary_Entry.json`

**What changed (high level)**
- Adjusted interaction chains so the primary use reliably:
  - Fires the hook projectile
  - Latches correctly to valid targets
  - Pulls the player or target as intended
- Cleaned up conditions/cooldowns to avoid:
  - “Dead” clicks where nothing happens
  - Stuck states where the hook stays unusable until relog

Result: **Hookshot and Longshot now behave consistently and feel usable in normal play.**

## 🛠️ Hylian Workbench fix

**Files changed**
- `mods/ZeldaGear-1.9/Server/Item/Items/Bench/Bench_Zelda.json`
- (plus any related registry/manifest entries already present in this mod)

**What changed (high level)**
- Applied SmileFGD’s community fix so that:
  - The Hylian Workbench item appears correctly in-game
  - Crafting/placement works as expected on a typical Hytale server

Result: **Hylian Workbench is now obtainable and functional using the bundled configs.**

