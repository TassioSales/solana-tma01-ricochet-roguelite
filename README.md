# 🎮 TMA-01: 9:16 One-Thumb Physics Ricochet & Merge Roguelite Mini-Game

Independent, single-file zero-dependency physics roguelite mini-game engineered for 9:16 mobile viewports and Telegram Mini Apps (TMA).

## 🚀 Key Features

- **Viewport & Aspect Ratio:** Locked 9:16 portrait canvas (360x640 logical, auto-scaling up to native DPR).
- **One-Thumb Physics Ricochet:** Aim trajectory projection with drag-and-release slingshot impulse.
- **Merge & Bounce Mechanics:** Ball-to-ball merge on threshold collisions, boundary reflections, and restitution damping.
- **Roguelite Card Drafting:** Post-wave dynamic 3-card perk selector (Multi-Shot, Plasma Trail, Kinetic Surge, Gravity Well).
- **Zero-Dependency Architecture:** Single standalone `index.html` file (HTML5 Canvas + vanilla ECMAScript 2022).
- **Deterministic Headless Test API:** Fully exposed `window.__GAME` harness:
  - `getState()`: Serializes balls, obstacles, score, wave, and perks.
  - `injectInput(action)`: Dispatches deterministic touch/mouse events.
  - `step(dt)`: Advances physics clock deterministically.
  - `triggerDraft(choiceIndex)`: Selects draft card programmatically.

## 🕹️ Quick Start

Open `index.html` directly in any modern browser or serve with:
```bash
npx serve .
```

## 🧪 Verification & Benchmarks

Run the automated verification suite:
```bash
node verify_tma01.mjs
```

## 📜 Bounty Details
- **Target Issue:** [incidere/solana-agent-bounties#13](https://github.com/incidere/solana-agent-bounties/issues/13)
- **Author:** [@TassioSales](https://github.com/TassioSales)
- **Solana Payout Wallet:** `DnkfGjiVZa5DKMNBkKMWciuzmZCVi1YD3Gw33cysF5hB`
