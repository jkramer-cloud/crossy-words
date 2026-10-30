# Crossy Words v2.6 — River Stability + Expanded Grammar Bank

A GitHub Pages-ready, single-file update of Crossy Words v2.5. This release keeps the existing 3D-style crossings, 48-row worlds, five grade bands, arcade/practice modes, coin earnings, capsule collection, and locally saved player progress.

## Install on GitHub Pages

1. Download and extract the release ZIP.
2. Open the **Crossy Words game** repository on GitHub.
3. Replace its root `index.html` with the included `index.html`.
4. Commit the changes. GitHub Pages will load the updated game at the same URL after it publishes.
5. Hard-refresh the page (Ctrl+Shift+R) if the old version remains cached.

This update does **not** require changing the Naches Learning Hub when the hub already links to the Crossy Words page. Do not replace your main Learning Hub `index.html` with the game file.

## Fixes and improvements

- **River fix:** Negative-direction rivers now use proper positive wraparound. At row 50 and other river rows, floating logs no longer vanish after long play sessions due to JavaScript's negative remainder behavior.
- **Expanded question bank:** 155 new curated items; total **359** questions. Distribution: 55 (grades 3–4), 107 (5–6), 106 (7–8), 45 (9–10), 46 (11–12).
- **Question rotation:** Each grade band receives a shuffled, nonrepeating deck of questions, refreshed only when exhausted. Prerequisite review questions (22% chance where applicable) use their own independent grade deck. The latest 20 questions are avoided when a deck cycles whenever possible.
- **Preserved systems:** Gameplay, grading-related grammar choices, character shop, cosmetics, saved stats, and modes remain available.

## Verification

Browser smoke tests checked all five grade-band counts, grade-deck nonrepetition, 501 world rows with a next question, and 270 river snapshots (rows through 499, elapsed play time 0–20,000 seconds). Every tested river snapshot had at least three visible log positions. No JavaScript page errors were reported in these tests.

Note: The tests are simulation-based, not a guarantee that every possible run or browser device is error-free. Please report the precise row, game mode, and circumstances if students encounter another obstruction.
