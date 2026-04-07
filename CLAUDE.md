# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

This is a single-file browser game — `kolko_i_krzyzyk.html` (Tic-Tac-Toe). No build tools, dependencies, or server required.

## Running

Open the file directly in any browser:

```
start kolko_i_krzyzyk.html
```

## Architecture

Everything lives in one HTML file:

- **HTML** — 3×3 grid of `.cell` divs, score display, status line, restart button
- **CSS** — dark theme, CSS Grid layout, win animation via `@keyframes pulse`
- **JS** — flat state (`board[]`, `current`, `gameOver`, `score`), win detection checks all 8 lines from `WINS` constant on every move
