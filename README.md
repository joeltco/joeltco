# Hi, I'm Joel 👋

Full-stack / systems engineer in **Detroit, MI**. I like building real things that ship and stay up.

### 🎮 [ff3mmo.com](https://ff3mmo.com) — a multiplayer NES game engine, from scratch

A browser-based **Final Fantasy III engine** with real-time multiplayer. No game framework, no copyrighted assets in the repo — it extracts everything from a user-supplied ROM at runtime. Live in production.

- **Server-authoritative architecture** — the server picks RNG seeds and monster pools and outcome-validates every battle, so the client can run combat locally at native speed without being able to cheat.
- **Real-time multiplayer over WebSockets** — presence, scoped chat, server-arbitrated PvP duels, and deterministic lockstep co-op battles with per-turn RNG resync to keep clients in sync across devices.
- **Hardened against hostile clients** — per-kind rate limiting, per-IP connection caps, payload clamping, JWT revocation + refresh, bcrypt timing equalization, protocol-boundary validation.
- **Headless test infrastructure** — a combat simulator running production code paths in Node, a wire-regression suite, and a load tester driving 200 concurrent clients against the real server.

`JavaScript (ES modules)` · `Node.js` · `Express` · `ws` · `better-sqlite3` · `JWT` · `bcrypt` · deployed on DigitalOcean

### 📈 tgoti — a "Tamagotchi for stocks" in your terminal

A Python TUI where each pet **is** a real brokerage position: HP tracks unrealized P&L, feeding buys shares, and pets age only during market hours.

- **Alpaca trading API** integration behind a clean abstraction with three runtime-swappable backends — sandbox / paper / live (dependency inversion).
- **203-file test suite** run in **CI across Python 3.11 & 3.12** with `ruff`, `mypy`, and `bandit` security scanning.
- ~50-module layered architecture (core / game / market / persistence / TUI).

`Python` · `Textual` · `Alpaca SDK` · `SQLite` · `pytest` · `GitHub Actions`

### 🛠️ Also

- **ebible-tui** — a typed, tested Python terminal app (Textual / Rich, mypy + pytest).

### 📫 Reach me

- 📧 joeltaylor734@gmail.com
- 💼 Open to software engineering roles (remote or Detroit area)
