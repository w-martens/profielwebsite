# Profielwebsite — W.A. Martens

## Stack

Plain static site: `index.html` + `style.css`. No build step, no framework, no package manager, no test runner, no CI.

## How to run

Open `index.html` in a browser directly, or serve with any static file server (e.g. `npx serve .`, `python -m http.server`).

## Design Principles
Do not invent layouts or visual styles unless explicitly asked.
Mockups inside /mockups are the source of truth.
Reproduce the mockups as accurately as practical.
If visual details are ambiguous, ask questions instead of guessing.
Use assets exactly as provided.
Preserve spacing, composition, proportions, and typography.

## Technology
Vanilla HTML
Modern CSS
Vanilla JavaScript (ES modules)
No frontend framework unless requested.
Minimize dependencies.
Prefer browser APIs over third-party libraries.

## Code Style
Keep files modular.
Prefer readability over cleverness.
Use descriptive names.
Avoid duplicate code.
Comment only where it improves understanding.
Keep CSS organized by component.

## Performance
Prioritize smooth animations.
Avoid unnecessary JavaScript.
Prefer CSS animations where appropriate.
Keep rendering efficient.
Avoid layout thrashing.
Optimize for modern desktop browsers first.

## Working Style

When implementing a feature:

Inspect the existing code.
Explain the proposed approach briefly.
Implement the feature.
Test it if possible.
Fix any issues before finishing.

## Design Ownership

The human decides:

layout
typography
colors
composition
iconography
illustrations
animation direction
overall artistic vision

The AI should avoid making aesthetic decisions unless explicitly requested.

## When Unsure

Prefer asking a question over making assumptions.

If a request conflicts with the mockups, ask which should take priority.

Never silently change the intended visual design.



## Structure

- `index.html` — page layout, inline JS (music note particles, color pickers, shatter nav animation). **Contains a second experimental glass UI appended below line 418** — two `<html>`/`<body>` roots in one file.
- `style.css` — CSS layers, `@property` for animated custom properties, local font faces.
- `fonts/` — TTF/OTF/FON files loaded by `style.css`.
- `img/` — PNG nav button images.
- `src/` — MP3 files (not yet wired up in the page).
- `aantekeningen.md` — Dutch-notes.md (idea backlog), not documentation.

## Conventions

- `opencode.json` configures the ponytail plugin — edits should prefer simpler over clever.
- No linter, formatter, or typechecker configured.
