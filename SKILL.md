# TRAC RUNNER — Skill File for Intercom Agents

## App Overview
TRAC RUNNER is a pixel-art platformer game (Super Mario-style) built as a single `index.html` file. It runs in any modern browser with zero dependencies.

## Agent Instructions

### How to Deploy
1. Clone this repo
2. Open `index.html` in a browser — no build step required
3. For hosting: upload `index.html` to any static host (GitHub Pages, Vercel, Netlify, etc.)

### How to Play (for agent automation)
- The game uses keyboard events: `ArrowLeft`, `ArrowRight`, `Space`, `ArrowUp`
- Touch events are supported for mobile agents
- Game state is exposed via `window.gameState` (values: `'playing'`, `'over'`)
- Score is in `window.score`, TNK in `window.tnk`

### Integration with Intercom
- This app can be extended to use Intercom sidechannels for:
  - P2P leaderboard sync between players
  - Real-time score broadcasting
  - Multi-agent coin placement coordination
- See [Intercom upstream](https://github.com/Trac-Systems/intercom) for P2P API

### File Structure
```
/
├── index.html     # Entire game (self-contained)
├── README.md      # Documentation + TRAC address
└── skill.md       # This file — agent instructions
```

## TRAC Network Context
This app runs on the Trac Network ecosystem. The in-game TNK currency mirrors the real TNK token concept, demonstrating gamified onboarding to the Trac Network.
