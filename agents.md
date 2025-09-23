# Agent Operating Guide

## Mission Context
- Maintain a catalog of one-page HTML5 games.
- Every game lives in a single self-contained HTML file (inline CSS/JS/assets).
- `index.html` lists and links to every game; update it whenever a new game ships.

## Current Repository Structure
- `README.md` — high-level project introduction.
- `agents.md` — agent-facing operating guide (this file).
- `copilot-instructions.md` — original instructions captured from the user.
- `index.html` — public landing page linking all games.
- `projectoverview.md` — goals, conventions, and dated Change log entries.
- `games/` — library of single-file games:
  - `cultivation-rpg.html`
  - `minesweeper.html`
  - `snake.html`
  - `tic-tac-toe.html`

## Core Responsibilities
1. **Plan First**: Document gameplay mechanics, controls, goals, and visual tone before writing code. Record the concept somewhere discoverable (e.g., project notes or a planning doc).
2. **Single-File Delivery**: Keep all code and assets embedded in the game file; avoid external networks or dependencies.
3. **Organized Repository**: Name game files clearly and keep the repo tidy so hosting is straightforward.
4. **Project Overview Hygiene**: Update `projectoverview.md` for any new game, structural change, or guideline adjustment. Add a dated Change log entry (date, author, short summary) and reference the file in commits/PRs.

## Standard Workflow
- Conceptualize and document the game idea.
- Implement the game in one HTML file.
- Add an entry to the index page pointing to the new game.
- Test the game locally; refine until it plays well.
- Update `projectoverview.md` with the latest changes.

## Working Tips
- Review `projectoverview.md` before editing to stay aligned with goals and conventions.
- Keep comments concise and only where they aid comprehension.
- When adding games, ensure styles/scripts do not leak globally—scope them within the single file.
- After changes, consider quick smoke tests (keyboard/mouse input, scoring, reset loops) to maintain playability.

## Communication
- When collaborating or committing, reference both the game file and the relevant `projectoverview.md` log entry so reviewers see the broader context.

Stay consistent with these practices to keep the game collection coherent and easy to maintain.
