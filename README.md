
# 🐍 Snake Game — Pure JavaScript

A fast, clean remake of the classic **Snake** using **HTML, CSS, and vanilla JavaScript**. Smooth controls, crunchy SFX, dynamic food & bombs, and a responsive layout that works on desktop and mobile.

[▶️ Play Demo](https://prashik24.github.io/SnakeGame/) 
• [📘 Tutorial](https://prashik24.github.io/SnakeGame/)

---

## ✨ Features

* **Classic Gameplay** — Eat food, grow longer, don’t crash.
* **Dynamic Spawns** — Randomized food and **bombs** (instant game over).
* **Robust Collisions** — Walls, self, and bomb detection.
* **Juicy Audio** — Bite, bomb, and game-over sounds (with toggle).
* **Responsive UI** — Scales nicely across devices.
* **(Optional)** High score saved with `localStorage`.

---

## 🎮 Controls

**Keyboard (Desktop)**

* `↑/↓/←/→` or `W/A/S/D` — Move
* `Space` — Pause / Resume
* `M` — Mute / Unmute

**Touch (Mobile)**

* On-screen arrows / swipe (if enabled)

---

## 🧠 Rules

* Eating food **+1 length** and **+score**.
* Hitting a **wall**, **yourself**, or a **bomb** ends the game.
* Speed may increase progressively (if enabled).

---

## 🚀 Quick Start

```bash
# 1) Clone
git clone https://github.com/prashik24/SnakeGame.git

# 2) Enter folder
cd SnakeGame

# 3) Play
# Option A: Open index.html in your browser
# Option B (recommended): run a static server for correct audio/asset loading
#   - VS Code: install "Live Server" → Right-click index.html → "Open with Live Server"
#   - Or using Python:
python -m http.server 8080
# then open http://localhost:8080 in your browser
```

> If your project lives elsewhere, replace the clone URL accordingly.

---

## 🧩 Tech Stack

* **JavaScript (ES6+)**
* **HTML5 Canvas**
* **CSS3**

---

## 📁 Project Structure (example)

```
SnakeGame/
├─ index.html
├─ css/
│  └─ styles.css
├─ js/
│  ├─ game.js          # main loop, game state
│  ├─ models/          # snake, food, bomb, grid utilities
│  └─ audio.js         # sfx/music helpers (if separated)
├─ images/             # icons, apple, bomb, etc.
└─ assets/             # audio files (if used)
```

---

## ⚙️ Configuration (optional)

You can expose simple tweakables in a `config` object (speed, grid size, bomb rate, sound enabled by default), e.g.:

```js
const CONFIG = {
  gridSize: 20,
  tickMs: 120,
  bombChance: 0.05,
  wrapAround: false,   // set true to allow going through walls
  soundEnabled: true
};
```

---

## 🧪 Development Tips

* Use a local server to avoid asset loading issues (audio/images).
* Keep update/draw cycles separate for readability.
* Debounce direction changes to prevent 180° turns in one tick.

---

## ❗ Troubleshooting

* **No sound?**
  Most browsers block autoplay. Interact (click/tap) once or toggle sound with **M**.
* **Black canvas or nothing happens?**
  Open via a local server (see Quick Start). Direct file URLs can block assets.
* **Controls feel laggy?**
  Close background tabs, reduce `tickMs`, or lower grid size.

---

## 🤝 Contributing

PRs welcome!

1. Fork the repo
2. Create a feature branch: `git checkout -b feature/my-feature`
3. Commit: `git commit -m "feat: add X"`
4. Push: `git push origin feature/my-feature`
5. Open a Pull Request

---

## 🗺️ Future Roadmap Idea :

* Difficulty modes (Easy/Normal/Hard)
* Skins & themes
* Power-ups (slow time, shield)
* Scoreboard with initials

---

## 📜 License

**MIT** — free to use, modify, and share.

---

## 🎯 Play Now

Dive in: [**SnakeGame Live**](https://prashik24.github.io/SnakeGame/)
Have fun, and don’t bite your tail!  keep Playing the Game have a fun guys 🐍✨

---
