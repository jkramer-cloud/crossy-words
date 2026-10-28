# Crossy Words — New Worlds & Clearer Landings (v2.2)

A free, single-file classroom grammar arcade game for grades 5–8, based on a student idea. Run through a scrolling pseudo-3D voxel world, select correct moving word platforms, dodge cars and occasional trains, cross rivers on logs, and use earned coins to unlock collectible characters.

## What changed in v2.2

- **Fixed overlapping sprites:** Characters are rendered once, with their feet and shadow aligned. The old doubled character artwork could make faces and limbs appear distorted.
- **Clearer hop destination:** A crosshair/ring sits on the *next row at the exact selected column*. A faint path connects the character to the intended landing spot. The marker predicts where a moving tile will be **when the hop finishes**. On small screens, a readable **Next Hop** status appears beneath the game board.
- **Landing guide colors:** Cyan = a word platform; red = missing platform/open water; green = safe ground/log; gold = a moving hazard that requires timing. **Cyan does not mean the grammar answer is correct.** Students must still read the question carefully. Traffic can change after landing, so students must keep moving.
- **12 map themes:** Sunny Meadow, City Streets, Punctuation Marsh, Snowy Summit, Neon Galaxy, Desert Dunes, Autumn Grove, Crystal Caves, Tropical Coast, Candy Valley, Bamboo Forest, and Volcanic Ridge. Each has distinct voxel scenery, such as city buildings, conifers, cacti, palm trees, glowing crystals, or bamboo. Worlds rotate after every 16 rows in a shuffled sequence.
- **Day/night scenes:** Each map can appear in daytime or a nighttime variation. At night, the sky darkens, stars and glowing environmental accents appear, and a soft glow surrounds the player's character. All scenes are rendered with built-in Canvas graphics—no images are downloaded.
- **360 collectible characters:** 12 new creature species—Deer, Panda, Slime, Bat, Cactus, Tiger, Octopus, Unicorn, Firefly, Astronaut, Hedgehog, and Jellyfish—have joined the existing 18 species. All 30 species have 12 palette variants and their own deterministic synthesized sounds.

## Existing features retained

- **Two modes:** Timed Arcade with fatal hazards; untimed Practice with coaching and nonfatal hazard rows.
- 98 curated grammar questions covering homophones, punctuation, verb tenses, agreement, parts of speech, and more, with different grade options.
- Moving word tiles with gaps, roads with 8 vehicle classes, occasional warning-signaled trains, and logs on rivers.
- Game-over snapshot, distance record, and personal best per equipped character.
- Gacha-style capsule machine using **earned in-game coins only** (80 coins each), no duplicates, no purchases or ads.
- Browser-local coins, unlocked characters, selected character, and scores. **Existing v1–v2.1 saves remain compatible on the same browser and origin.**

## Controls

- **Left/Right arrows** or **A/D** move sideways among five columns.
- **Up arrow**, **W**, **Space**, or the **HOP** button moves forward one row.
- Tap an answer in the strip below the board to aim at an available matching tile, then press HOP when ready. A word button does **not** hop automatically.
- The marker predicts the *surface* under the target location at touchdown. It does not reveal which word is grammatically correct.
- Stop on safe rows to observe vehicles and railroad signals; avoid lingering on roads.

## GitHub Pages installation

To update an existing `crossy-words` repository, upload this package's **`index.html`** to the repository root, replacing the existing `index.html` file. You can update `README.md` as well. The URL stays the same, so the Learning Hub card does not need an update.

For a new repository: create `crossy-words`, upload both files, and enable **Settings → Pages → Deploy from a branch → main → / (root)**.

## Technology and privacy

The entire app runs in standard HTML, CSS, Canvas 2D, and JavaScript. It uses no AI service, API key, third-party dependency, server, account, or tracking code. Character audio is synthesized in the browser and may be muted. Data is saved only in the local browser using `localStorage`; progress is not synced between devices or incognito sessions.

The perspective view is **2.5D** (depth-rendered Canvas), not actual WebGL 3D. The extra animals are procedurally illustrated, not individual downloadable 3D models.
