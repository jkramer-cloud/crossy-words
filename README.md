# Crossy Words — v2.3: Longer Worlds & New Hoppers

A no-login, browser-based grammar arcade game for **grades 3–12**. It combines five-column hopping, moving word platforms, traffic, log crossings, occasional trains, a coin economy, and capsule unlocks.

## Install on GitHub Pages

1. Create or open your existing `crossy-words` GitHub repository.
2. Put `index.html` in the **repository root** (replace the old `index.html`).
3. Optionally upload this `README.md`.
4. In **Settings → Pages**, deploy from `main` and `/ (root)`.
5. The site URL remains `https://jkramer-cloud.github.io/crossy-words/` if using that account and repository name. No Learning Hub URL change is needed.

## What's new in v2.3

- **48 rows per environment**, three times v2.2's 16 rows. A progress meter shows how far you have explored before the theme changes.
- **16 map environments** (up from 12): four new themes are Cloud Kingdom, Coral Reef, Moon Base, and Clockwork Yard. Each environment can appear in daytime or with night effects and glowing props.
- **576 character variations** across 48 types and 12 color styles. Newly added 18 character types include Mini Giraffe, Lumberjack, Griffin, Wizard, Pirate, Knight, Butterfly, Chef, Explorer, Phoenix, Robot DJ, Fairy, Snow Yeti, Firefighter, Pilot, Forest Sprite, Space Ranger, and Peacock. Wing and tail shapes are drawn into the procedural artwork.
- **Random equip** selects a different *already unlocked* character without a coin cost. It works from the sidebar and the collection menu; it never grants a locked one.
- **Five grade bands:** 3–4, 5–6, 7–8, 9–10, 11–12. The game includes 204 carefully written grammar questions and brief explanations. Questions are drawn mainly from the selected grade band, with occasional review of the immediately lower band.
- **Grade-adjusted arcade timers:** the youngest students have more reading time, and older high-school levels allow time for more sophisticated questions. Practice mode remains untimed.

## Core controls

- Left / A: move left
- Right / D: move right
- Up / W / Space: hop forward
- Tap an option to line up with an available moving tile, then time the hop
- Pause button pauses active gameplay
- A colored landing ring and Next Hop label help identify the landing surface; they do not reveal the correct answer

## Saved progress

Progress, coins, character unlocks, equipped character, high scores, and preferences use the browser's local storage key `crossy_words_hopper_save_v1`. The updated game intentionally retains that key so existing local saves can carry over, provided students continue using the same browser and origin. Clearing site data, using another device, or private browsing can lose the save. **No student information is sent to a server.**

## What the physics checks mean

This is a fast arcade game, not a formal grammar assessment. The built-in questions are authored locally. All roads, moving platforms, logs, and train hazards still use simplified arcade collision and movement rules. The same character collection works across all grade bands; cosmetic rarity doesn't provide an advantage.

## Development/testing

Verified with Chromium automated checks for five grade choices, character counts and random equip, 48-row map boundaries, gallery rendering, basic gameplay initiation, and phone-width layout without horizontal overflow. Browser audio may require an initial click due to autoplay restrictions.
