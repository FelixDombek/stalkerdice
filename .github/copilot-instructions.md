# GitHub Copilot Instructions

## Project Overview

**stalkerdice** is a browser-based dice roller for the [STALKER board game](https://felixdombek.github.io/stalkerdice/), which is based on the *S.T.A.L.K.E.R.* video game series set in the Chernobyl Exclusion Zone.

## Tech Stack

- **Pure HTML/CSS/JavaScript** – single file (`index.html`), no build system, no dependencies, no package manager.
- **GitHub Pages** – the app is deployed directly from the repository root.

## Key Files

| File | Purpose |
|------|---------|
| `index.html` | The entire application: HTML structure, CSS styles, and JavaScript logic |
| `README.md` | Project readme with live demo link |
| `suggestions.md` | Backlog of improvement ideas |
| `.github/workflows/pr-preview.yml` | Deploys PR preview pages via `rossjrw/pr-preview-action` |

## Game Rules Context

The STALKER board game uses two types of custom six-sided dice:

**Green dice** (6 faces):
- ★★ (weighted/special – counts as +2 weighted stars)
- ★★★
- ★★
- ★
- ★
- *(blank)*

**Yellow dice** (6 faces):
- ☠☠ (2 gas masks)
- ★☠ (1 star + 1 gas mask)
- ★☠ (1 star + 1 gas mask)
- ★★ (2 stars)
- ☠ (1 gas mask)
- ★ (1 star)

Stars (★) are successes; gas masks (☠) are a hazard resource. The "weighted" green face has a white inner square and counts as extra stars in certain game contexts.

## Coding Conventions

- All logic lives in `index.html` – keep it that way; do **not** split into separate `.js` or `.css` files unless explicitly asked.
- CSS classes follow BEM-ish naming: `.die`, `.green-die`, `.yellow-die`, `.face-0`…`.face-3`, `.weighted-face`, etc.
- JavaScript uses plain `const`/`let`, arrow functions, template literals – ES6+ is fine; no TypeScript.
- No external libraries or CDN links.

## How to Test

Open `index.html` directly in any modern browser – no server needed. There are no automated tests.

## Deployment

Merging to `main` automatically deploys to <https://felixdombek.github.io/stalkerdice/> via GitHub Pages. Pull requests get a live preview URL posted automatically by the CI workflow.
