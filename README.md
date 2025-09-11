# Steps — React Component

A simple, focused React UI to guide users through a 3‑step flow. The design features circular step indicators, a collapsible panel, and clear Previous/Next navigation. Built as part of a React learning series.

## Features

- Step indicators: three numbered circles with active highlighting
- Collapsible panel: toggle visibility with a close button (×)
- Navigation: Previous/Next buttons with bounds checking
- State management: `useState` for step and open/close state
- Styles: minimal, accessible defaults in `src/index.css`

## Quick Start

Prerequisites: Node.js 18+ and npm.

- Install: `npm install`
- Develop: `npm start` (opens at http://localhost:3000)
- Test: `npm test`
- Build: `npm run build` (outputs to `build/`)

## Project Structure

- `src/App.js`: Main `Steps` component and app shell
- `src/index.js`: App bootstrap and StrictMode
- `src/index.css`: Styles for steps, buttons, and layout
- `public/`: Static assets and HTML template

## Design Notes

- Visual style: neutral container (`#f7f7f7`) with accent color `#7950f2`
- Step UI: three equal circles; active step in white-on-accent
- Layout: numbers at top, message centered, actions spaced left/right
- Toggle: close button in the top-right to collapse/expand the panel

## Customization

- Steps/messages: edit the `messages` array in `src/App.js`
- Colors/spacing: adjust tokens in `src/index.css`
- Behavior: update `handlePrevious`/`handleNext` and step bounds

## Accessibility

- Keyboard: buttons are reachable via Tab; focus styles rely on browser defaults
- Labels: buttons use clear text; consider adding `aria-label` for the close button
- Future: announce step changes via `aria-live` region if needed

## Scripts

- `npm start`: Run a local dev server with fast refresh
- `npm test`: Run tests in watch mode (if/when added)
- `npm run build`: Create an optimized production build in `build/`

## Notes

This project was scaffolded with Create React App and then adapted to the new Steps design for clarity and focused practice.
