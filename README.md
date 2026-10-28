# Crossy Words — v2.4 Arcade Academy

A browser-based grammar hopping game for grades 3–12. Dodge traffic and trains, time moving word platforms, collect characters, and practice grammar. No AI, sign-in, external APIs, or payments are required.

## Install on GitHub Pages

1. Open your existing `crossy-words` repository.
2. Replace the old `index.html` with the `index.html` in this ZIP. You can also replace `README.md` and add `CHANGELOG.md`.
3. Commit to the published branch. GitHub Pages will serve the updated game at the same address: `https://jkramer-cloud.github.io/crossy-words/`.
4. Students might need to refresh the page after deployment.

To play offline, download and open `index.html` in Chrome or Edge. This is one self-contained file.

## What is new in v2.4

### Independently adjustable Arcade difficulty

**Grammar grade** determines question content (3–4, 5–6, 7–8, 9–10, or 11–12). It does not determine arcade difficulty.

**Explorer**: 32% slower cars, one fewer car per traffic row, slower word tiles, rarer/slower trains, and 35% more time than Standard.

**Standard**: the original balanced speeds and timers.

**Expert**: 38% faster traffic, an additional car per road, faster word tiles and trains, more trains, and 18% less time.

These presets apply to Arcade mode. Practice mode remains untimed and disables fatal traffic hazards so students can focus on grammar.

### Challenges and persistent badges

- **11 general achievements** reward grammar practice, combos, travel, night maps, safe Arcade crossings and collecting characters.
- **3 challenges per world**: answer 5 grammar questions, survive 6 obstacle rows in Arcade mode, and complete that 48-row region.
- There are 16 worlds, so 48 world badges are available.
- Challenge progress within a world is per-run. Awarded badges and their coin rewards persist on that browser. A badge can pay out only once per world.
- View current challenge progress in the sidebar or open **View all achievements** to browse the full collection.

### Learn from missed grammar answers

- A grammatical mistake or grammar timeout in Arcade mode opens a **Mini Grammar Retry** on the results screen. Choose one of the sentence options, then receive an explanation of the correct answer before restarting.
- In Practice mode, incorrect choices show a clear correction in the Word Coach panel and let the student try again without ending the run.
- Vehicle crashes, missed logs, and other timing failures remain separate from grammar mistakes.

### Features retained from v2.3

- 576 collectible character color/creature combinations with synthesized sounds and a no-duplicate capsule shop.
- Random equip from unlocked characters.
- 16 map regions, 48 rows per region, with day and night variants.
- 204 original grammar items across five grade bands.
- Moving traffic, trains, rivers, word platforms, visual landing guide, and results snapshots.

## Controls

- Left / Right arrow keys, or A / D: move one of five columns.
- Up arrow, W, or Space: hop forward.
- P / Escape: pause.
- On-screen directional buttons also work on touchscreen devices.
- Tap answer tiles on the option bar to line up under a matching word platform. Wait until the moving word reaches a landing spot, then hop.

## Progress and privacy

Progress is saved in **localStorage** under `crossy_words_hopper_save_v1`. The same storage key is used as previous versions so previously unlocked characters, currencies and records are retained. New badges and difficulty preferences are added without resetting existing records.

Data stays on the user's device/browser. Clearing browser storage or opening the game on another device will not carry over progress. The game uses no accounts, trackers or AI services. The stress of real-time Arcade mode can be reduced using **Explorer** or the untimed **Practice** mode.

## Notes for educators

The questions come from a curated offline bank, so text is not analyzed by an AI. Grammar feedback is tied to the stored explanation for each item. The game is designed as grammar practice, not a comprehensive assessment of all ELA standards.
