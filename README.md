# ⎈ HELM — Paper Trading Simulator for Solana Memecoins

**Learn. Train. Trade. Zero risk.**

HELM is a free, browser-based paper trading simulator designed to help newcomers learn memecoin trading without losing real money. Analyze real tokens with live data, practice buying and selling with simulated SOL, and build your skills before entering the trenches.

> *"If this had existed when I started, I would've saved a lot of SOL."*

---

## Why HELM?

Crypto Twitter extracts too much from newcomers. Most people lose everything on their first trades because nobody teaches the basics — they're thrown straight into the fire.

HELM exists to change that. Whether you're learning to trade or teaching others, HELM gives you a risk-free environment to develop real skills with real market data.

---

## Features

### 🔍 Token Analysis
- Paste any Solana token address and get instant analysis using live DexScreener data
- **Red flags** — rug risk, wash trading, low liquidity, sniper wallets, honeypot patterns
- **Green flags** — healthy MC, good holder distribution, verified socials, locked liquidity
- Risk score (0-100) with severity levels: Low, Medium, High, Extreme
- Direct links to DexScreener charts, Telegram, Twitter, and project websites

### 📊 Paper Trading
- Start with **5 SOL** (simulated) — no real money involved
- **Buy (APE)** — enter positions on analyzed tokens
- **DCA** — dollar cost average into existing positions
- **Partial Sell** — take profits at any percentage
- **Close Position** — full exit with P&L calculation
- **Realistic slippage** — simulated based on actual 24h volume (0.2% to 4%)
- Live price updates from DexScreener API

### 📖 Education
- **41-term glossary** covering Trading, On-Chain, CT Culture, and Risk categories
- Searchable glossary with category filters
- **Contextual tooltips** — technical terms in analysis flags are tappable, showing instant definitions
- **Post-trade tips** — educational feedback after every closed position based on your performance
- **Guided starter flow** — 5-step onboarding that walks new users through their first analysis and trade
- **BubbleMaps guide** — learn to read wallet distribution and spot insider clusters

### 🏆 Gamification
- **XP system** — earn XP from trades, missions, and community activity
- **10 levels** — Normie → Observer → Ape → Degen → True Degen → Diamond Hands → Master Degen → Whale → Alpha Caller → Insider
- **Badges** — First Trade, First Win, Hot Streak (3/5/10), Win Rate milestones (50%/60%/70%), and more
- **Win/loss streaks** — bonus XP for consecutive winning trades

### 🌐 Community
- **6 topic channels** — Tips/Tutorials, Rug Alerts, KOLs, News, Calls, Whales
- Post analyses, share calls, warn about rugs
- Like and report system with auto-moderation
- **Expiring posts** — Calls and Whale alerts expire in 24h, Rug alerts in 48h, News in 72h
- Community reputation ranking

### 📈 Ranking
- Global leaderboard ranked by XP
- Shows level, total P&L, win rate, and trade count
- Weekly narrative voting — the community votes on which narrative is trending

### 🎯 Missions & Rewards
- **Post in Community** — earn 0.2 SOL per post (max 3/week)
- **Login Streak** — 0.5 SOL for 3-day streak
- **Invite a Friend** — 0.5 SOL reward
- **Watch Ads** — 0.2 SOL per simulated ad (max 3/day)
- Bankrupt recovery system — if you lose everything, missions let you earn SOL back

### 🎨 Themes
- **Default** — dark theme
- **Light** — clean light mode
- **Neon** — cyberpunk vibes

### 📱 Responsive
- Fully optimized for mobile and desktop
- Touch-friendly interface

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | React 18 (createElement, no JSX) |
| Auth | Supabase (email + password) |
| Database | Supabase (PostgreSQL) |
| Market Data | DexScreener API |
| SOL Price | CoinGecko API |
| Charts | Chart.js |
| Deployment | Single HTML file |

---

## Project Structure

The app is built as a single-page HTML application. For development, the codebase is split into logical modules:

```
index.html                    # Complete production build (single file)
parte1-head-css-config.html   # HTML head, CSS, theme config
parte2-auth.js                # Supabase auth, AuthScreen, AuthWrapper
parte3-modais-trade.js        # Trade modals (buy, DCA, partial sell, close)
parte4-ranking-community.js   # Ranking board, community posts, comments
parte5-modais-info.js         # Info modals, starter flow, weekly report
parte6a-logica.js             # Core logic (trades, XP, missions, analysis)
parte6b-render1.js            # Render — header, tabs, analysis, portfolio
parte6c-render2.js            # Render — profile, settings, learn section
```

---

## Getting Started

1. Open `index.html` in any modern browser
2. Create an account (email + password)
3. Choose your username
4. Follow the starter flow or jump straight into analysis
5. Paste any Solana token address → Analyze → Trade

No build step. No dependencies to install. No wallet to connect.

---

## Roadmap

HELM is day 1. The app will keep evolving based on community feedback. Planned improvements include:

- [ ] Real-time price tracking for open positions
- [ ] Advanced analytics (Sharpe ratio, max drawdown, risk-adjusted returns)
- [ ] Social features (follow traders, copy paper trades)
- [ ] Mobile app (PWA)
- [ ] Token screener with filters
- [ ] Trading journal with export
- [ ] Multi-chain support
- [ ] AI-powered trade analysis feedback

---

## Contributing

Feedback, bug reports, and feature requests are welcome. Open an issue or reach out on X.

---

## License

This project is proprietary. All rights reserved.

---

**Built for the trenches. By someone who's been there.** ⎈
