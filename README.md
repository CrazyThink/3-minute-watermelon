# 🍉 3-Min Watermelon (3분수박)

**English** | [한국어](README.ko.md)

### ▶️ Play now: **https://crazythink.github.io/3-minute-watermelon**

A cute, juicy **Suika-style fruit-merge game** crossed with a **roguelike + Balatro-style score engine** — all in a **single HTML file**, no build step, no dependencies.

Drop fruits, merge matching ones, build wild score multipliers, and chase a high score before the **3-minute** timer runs out.

> Play offline by just opening one file. Korean / English / Japanese supported.

---

## ✨ Features

- **Suika-style physics merge** — round cute fruits with a custom fixed-timestep collision solver (no tunneling, no infinite rolling, natural piling).
- **Balatro-style score inflation** — score = `chips × multiplier`. Stack combos, passives, golden touch and fever for explosive scores (1M is normal, 100M+ is a great build).
- **Roguelike cards** — level up to pick from 5 grades of ability cards (Common → Mythic), with paid **reroll** (free rerolls via upgrades).
- **3 game modes**
  - 🍉 **Classic** — merge small fruits up; upgrades & items enabled.
  - 🔁 **Reverse** — start from watermelon, merge *down* — the **smaller** the fruit, the **higher** the score.
  - 📅 **Daily** — a date-seeded run with the same fruit order for everyone, no upgrades/items, for a fair daily best.
- **Meta progression** — earn coins to buy permanent **upgrades**, consumable **items**, cosmetic **background themes**, and a repeatable **Prestige** (permanent score multiplier).
- **Records** — lifetime **stats**, coin-rewarding **achievements**, and daily **missions** + streak rewards.
- **Card Codex** — browse every card and its drop rate by grade.
- **Polish** — synthesized WebAudio BGM (calm menu track / energetic in-game track) + SFX, mobile haptics, fireworks on a new record, score-milestone callouts, auto-pause on tab blur, and a shareable result card.
- **Multi-language** — 🇰🇷 한국어 / 🇬🇧 English / 🇯🇵 日本語, switchable in-game (🌐).
- **Responsive** — works on desktop and mobile (portrait) layouts.

---

## ▶️ How to Play

- **Click / tap** in the box to drop the current fruit.
- Two **identical fruits** that touch **merge** into the next one (Classic) or the previous one (Reverse).
- **Don't let fruits pile above the red line** — if they stay over it too long, it's game over.
- **Level up** by merging to pick an ability card.
- Survive and score as high as possible within **3 minutes** (the analog clock fills once per 3 min, then overflows in teal).

---

## 🚀 Play / Run

**▶️ Just play in your browser: https://crazythink.github.io/3-minute-watermelon**

Prefer to run it yourself? It's a single static HTML file — no install, no build.

**Option A — open the file directly**

```
open index.html      # macOS
# or double-click the file in your file manager
```

**Option B — local web server** (recommended; some browsers restrict audio/storage on `file://`)

```bash
python3 -m http.server 8765
# then visit http://localhost:8765/
```

Hosted on **GitHub Pages** (the file is `index.html`, so it serves straight from the repo root). Any static host (Netlify, etc.) works too — just upload the files.

---

## 🛠 Tech

- **Vanilla JavaScript** + HTML5 **Canvas** — no framework, no bundler.
- **WebAudio API** — all music & sound effects are synthesized at runtime (no audio assets).
- **localStorage** — saves best score, coins, upgrades, items, themes, prestige, stats, achievements, daily progress, and language/audio settings.
- **Google Fonts**: `Jua`, `M PLUS Rounded 1c`, and `Nunito` (the only external resources).

Everything (HTML, CSS, JS, game data, translations) lives in `index.html`.

---

## 🌐 Internationalization

The UI, cards, upgrades, missions, achievements, themes and tooltips are fully translated into **Korean, English, and Japanese**. Language is stored in `localStorage` and the browser language is auto-detected on first run. Add a language by extending the `TR` dictionary and the per-data translation entries.

---

## 📁 Project structure

```
.
├── index.html              # the entire game (open this)
├── apple-touch-icon.png    # home-screen / favicon icon
├── og-image.jpg            # Open Graph share image
├── README.md               # English README
└── README.ko.md            # Korean README (한국어)
```

---

## 📜 License

Released under the **MIT License** — free to use, modify, and distribute. See `LICENSE` (add one when publishing).

**Fonts:** `Jua`, `M PLUS Rounded 1c`, and `Nunito` are provided by Google Fonts under the **SIL Open Font License (OFL)** and are free for commercial use. Emoji are rendered by the operating system and are not bundled.

---

## ☕ Support

If you enjoy the game, you can support development here:
**[buymeacoffee.com/crazythink](https://buymeacoffee.com/crazythink)**

---

© 2026 CrazyThink.
