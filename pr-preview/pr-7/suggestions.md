# Suggestions for Evolving the STALKER Dice Roller

This file collects ideas for improving and expanding the dice roller app for the STALKER board game (based on the *S.T.A.L.K.E.R.* video game series set in the Chernobyl Exclusion Zone).

---

## Visual Improvements

- **Dice face images** – *(Partially done: each rolled die is now shown as a styled tile with ★/☠ symbols matching the physical face.)* Take this further with pixel-art or illustrated images of the actual STALKER dice faces to more closely match the physical board game experience.
- **Animated dice roll** – Add a short CSS/JS animation of the dice tumbling before showing the result, increasing the tactile feel of rolling.
- **Dark Zone theming** – Lean further into the S.T.A.L.K.E.R. aesthetic with distressed fonts (e.g. `VT323` or `Share Tech Mono`), a radioactive-green glow, and a background image or texture resembling the Chernobyl Zone.
- **Sound effects** – Play a dice-clatter sound on roll and a Geiger counter click when a gas mask result appears.

---

## Gameplay Features

- **Multiple dice sets** – Some encounters call for different dice pools (e.g. a black/skull die for dangerous anomaly zones). Add a third die type with its own face distribution.
- **Preset buttons** – Quick-select buttons for common rolls described in the rulebook (e.g. "Anomaly Check", "Mutant Attack", "Artifact Search") that pre-fill the correct number of green and yellow dice.
- **Roll history** – Keep a short log of the last 5–10 rolls so players can review what happened during a turn.
- **Probability / statistics panel** – *(Done: a "Mean per roll" bar at the bottom shows the expected stars, weighted stars, and gas masks for the selected dice pool.)* Could be extended with a full probability distribution (histogram or percentile table) for more analytical players.
- **Re-roll mechanic** – Allow individual dice to be re-rolled (some cards in the game grant a re-roll) while keeping the rest of the result.

---

## Accessibility & Usability

- **Mobile-first layout** – The app is already usable on mobile, but larger touch targets for the die-selector squares and a sticky "Roll" button at the bottom of the screen would improve one-handed play.
- **Keyboard shortcut** – Press `Space` or `Enter` to roll, useful for quick play during a session.
- **PWA / offline support** – Add a `manifest.json` and a simple Service Worker so the app can be installed on a phone's home screen and used without an internet connection at the table.
- **Localisation** – Provide translations for German, Russian, and Polish, as these are common languages in the STALKER fan community.

