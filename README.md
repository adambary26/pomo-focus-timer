# Pomo — Focus Timer

[![Live Demo](https://img.shields.io/badge/demo-live-58cc02?style=flat&logo=githubpages)](https://adambary26.github.io/pomo-focus-timer/)

> A cozy, Apple-style Pomodoro timer with an animated sky, ambient music, 11 theme palettes, task management, and session tracking.

![Pomo App Preview](https://raw.githubusercontent.com/adambary26/pomo-focus-timer/main/candle.png)

---

## ✨ Features

- **Pomodoro Timer** — 25 min work / 5 min short break / 15 min long break with custom durations
- **Task List** — add, check off, and delete tasks during your focus sessions
- **Session Stats** — pomodoro count + total focus time tracked
- **Skip with Options** — skip to next phase with Count (saves the pomodoro) or Discard (ignores it)
- **Sound Notification** — soft beep when a session ends
- **11 Theme Palettes** — Tech, Sunset, Ocean, Forest, Lavender, Midnight, Cherry, Desert, Neon, Mono, Aurora — changes accent, sky gradient, and break color
- **Dark Mode** — toggle sun/moon icon, persisted across visits
- **Ambient Music** — Rain, Forest Birds, and Lo-fi Study sounds with volume control
- **Animated Sky** — drifting clouds on a gradient sky that changes with theme
- **Apple Glass Design** — pill buttons, translucent blur cards, thin borders, subtle shadows
- **Plus Jakarta Sans** — modern bold font (700/800 weight) throughout
- **localStorage Persistence** — timer settings, tasks, stats, theme, and palette survive page refresh

---

## 🖼 Design System

| Token | Value |
|---|---|
| Font Display | Plus Jakarta Sans 800 |
| Font Body | Plus Jakarta Sans 700 |
| Border Radius | 8px (cards 20px, buttons 9999px) |
| Backdrop Blur | 16px (cards), 24px (buttons) |
| Sky | Animated gradient with 5 drifting clouds |

### Palette Architecture

Each theme sets 6 CSS custom properties via `data-palette` attribute:
- `--accent` — primary CTA color
- `--break-color` — break phase accent
- `--sky-top` / `--sky-bottom` — sky gradient stops

Default palette: **Tech** (`oklch(58% 0.16 145)` — green).

---

## 🧠 How to Use

1. **Start a session** — click the green Start button (pauses/resumes)
2. **Work** until the timer runs out — you'll hear a soft beep
3. **Break** — the timer auto-switches to short or long break
4. **Skip** — use Skip + Count/Discard to jump phases
5. **Track tasks** — add tasks in the sidebar, check them off as you go
6. **Change themes** — click a palette dot in the sidebar to change the look instantly
7. **Play music** — select Rain / Forest / Lo-fi and hit Play
8. **Dark mode** — click the sun/moon icon top-right
9. **Settings** — gear icon opens custom durations (work, short break, long break, interval)

---

## 🔧 Tech Stack

- **Vanilla HTML / CSS / JavaScript** — no framework, no build step
- **CSS Custom Properties** — OKLch color space for harmonious palette generation
- **Web Audio API** — beep notification
- **localStorage** — state persistence
- **HTML5 `<audio>`** — ambient sound playback

---

## 🚀 Live Demo

[https://adambary26.github.io/pomo-focus-timer/](https://adambary26.github.io/pomo-focus-timer/)

---

## 📁 Project Structure

```
.
├── index.html      # Single-file app (all CSS + JS inline)
├── candle.png      # Logo icon (28×28)
├── README.md       # This file
└── (backup files)
    ├── pomo-focus-timer.html
    ├── pomo-focus-timer-2.html
    └── ...
```

---

## 📄 License

MIT — use it, tweak it, ship it.

---

*Built with focus, one pomodoro at a time.*
