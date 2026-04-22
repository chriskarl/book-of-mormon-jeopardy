# Book of Mormon Jeopardy

A browser-based Jeopardy-style trivia game for Family Home Evening, youth activities, firesides, or any gathering where folks want to test their knowledge of the Book of Mormon.

**Live:** https://bom-jeopardy.netlify.app *(pending first deploy — see below)*

Companion to [Your March](https://peppy-squirrel-88ede7.netlify.app), the 100-day Book of Mormon reading challenge. Same visual family, same spirit.

## Features

- **6 × 6 board** — 6 categories (People, Places, Doctrine, Events, Faith, Repentance) × 6 questions, 100–600 points with a graduated difficulty ramp (600 is genuinely challenging).
- **36 seed questions** drawn from the title page through Alma 32 — all fully editable.
- **4 teams** with inline-editable names, live score tracking, and quick +100 / −100 / reset-to-zero buttons for mid-game corrections.
- **Hint button (½ points)** — if nobody can answer, reveal a hint. The next team to answer correctly earns half points; a wrong answer after the hint loses half.
- **Answer Key view (host only)** — opens a phone-friendly answer sheet in a new tab so the host can run the game confidently even without every answer memorized. Prints cleanly too.
- **Edit mode** — rewrite any category title, clue, or answer. Designed to be reused for different activities (not just Book of Mormon).
- **Export / Import JSON** — save a configured game and share it.
- **Persistent** via `localStorage` — scores and edits survive page reloads.
- **Single file** — no build step, no dependencies beyond Google Fonts (Oswald + Source Serif 4).

## Running locally

Open `index.html` in any modern browser. That's it.

## Deploying (Netlify)

This repo is set up for zero-config Netlify deployment:

1. Log into [Netlify](https://app.netlify.com)
2. **Add new site → Import an existing project → GitHub**
3. Pick this repo
4. Build command: *(leave blank)* · Publish directory: *(leave blank or `.`)*
5. Deploy. Rename the subdomain (e.g., `bom-jeopardy`) under **Site settings → Domain management**.

Every push to `main` auto-deploys.

## How to host a game

1. Click **Answer Key** in the top bar → opens a private answer sheet in a new tab. Copy the URL to your phone, or click Print → Save as PDF → AirDrop to your phone.
2. On the main screen, click any tile to read the clue to the room.
3. When a team answers, click their chip → **Right** (+points) or **Wrong** (−points). Wrong keeps the tile open for another team to buzz in.
4. If the question is too hard, click **Show hint (½ pts)** → the next right/wrong answer awards or deducts half.
5. Edit team names inline at any time. Use per-team +100 / −100 / 0 buttons for mid-game corrections.
6. **New game** resets scores and tiles but keeps your questions. **Reset** restores the seed Book of Mormon set.

## Design credit

Color system, typography, and Mesoamerican motifs are lifted directly from [Your March](https://peppy-squirrel-88ede7.netlify.app) so the two apps feel like members of the same family.

## License

MIT — feel free to fork for your ward, stake, or family.
