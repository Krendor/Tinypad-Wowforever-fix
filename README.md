# TinyPad – WoW: Forever Compatibility Patch

This repository contains only the two modified files (`TinyPad.toc` and `main.lua`) needed to make **TinyPad** run on **World of Warcraft: Forever** without Lua errors.

## Credit & Attribution
* **Original Addon Author:** **Gello**
* **Project Identifiers:** CurseForge ID `84962` / Wago ID `RqGZpQ6d` / WoWI ID `4417`
* This is a free, community compatibility fix for **WoW: Forever** and is not affiliated with or endorsed by the original author or Blizzard Entertainment.

## What Was Changed
1. **`TinyPad.toc`**: Updated `## Interface:` to `16001` so the client recognizes the addon for WoW: Forever.
2. **`main.lua`**: Added a safe fallback helper for mouse-over checks (`MouseIsOver` / `frame:IsMouseOver()`) to prevent `attempt to call a nil value` in `UpdateFadeBehavior` and `OnUpdate`, and fixed a `fadeTimer` reset typo.

## How to Install
1. Download and install the original **TinyPad** addon from its official page first.
2. Copy `TinyPad.toc` and `main.lua` from this repository into:
   `World of Warcraft\_forever_\Interface\AddOns\TinyPad\`
3. Overwrite the two existing files when prompted, then start or `/reload` the game.