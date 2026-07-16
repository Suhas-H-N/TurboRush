# 🚗 NeonDrive — Arcade Racer

> Perspective-road arcade car game. Dodge traffic, collect power-ups, chase high scores.  
> Pure HTML + CSS + Canvas. No libraries. No install. Just open and play.

---

## 🚀 How to Play

**Double-click `index.html`** — runs in any modern browser. No server needed.

---

## 🎮 Controls

| Input | Action |
|-------|--------|
| ← → Arrow Keys | Change lane |
| A / D | Change lane |
| P / Escape | Pause |
| Left/Right buttons | Mobile steering |
| Swipe left/right | Mobile lane change |

---

## 📁 Files

```
cargame/
├── index.html   ← All screens: title, game, game over, how-to, leaderboard
├── style.css    ← Full dark neon design system
├── game.js      ← Complete game engine
└── README.md
```

---

## ✨ Features

### 🎨 Visuals
- **Forced-perspective road** — pseudo-3D vanishing point illusion with animated lane markings
- **Procedural city skyline** — silhouetted buildings with lit windows that scroll in parallax
- **Star field** — twinkling background stars with sine-wave opacity animation
- **Detailed pixel-art cars** — player car and obstacle cars drawn entirely on Canvas with gradients, windows, wheels, lights
- **Particle system** — explosions on collision, collect bursts on power-ups, speed sparks, boost trail
- **Neon glow effects** — CSS `text-shadow` and Canvas `shadowBlur` throughout
- **Title screen animation** — live animated road with atmosphere cars playing in background

### 🏎️ Gameplay
- **5 lanes** — full-width perspective road with smooth lane-change transitions
- **Escalating difficulty** — speed and spawn rate increase every 500 points
- **3 shield health system** — colour-coded health bar (green → yellow → red)
- **Dodge streak combos** — 5, 10, 15, 20+ dodge chains multiply score
- **Score multiplier** — base ×1, combo ×2–5, boost power-up ×2

### ⚡ Power-Ups
| Power-Up | Effect | Duration |
|----------|--------|----------|
| 🛡 Shield | +1 HP (max 3) | Instant |
| ⚡ Boost | 2× score multiplier | 5 seconds |
| 🧲 Magnet | Auto-attract nearby power-ups | 3 seconds |
| ⭐ Star | Full invincibility | 4 seconds |

### 🏆 Screens
- **Title** — animated road background, best score display, menu navigation
- **Game** — HUD with score, speedometer arc, distance, level, health bar, active power-up timers
- **Game Over** — full stats breakdown (score, distance, top speed, level, dodge streak, new best indicator)
- **How To Play** — controls and mechanics guide
- **Leaderboard** — top 20 scores with gold/silver/bronze medals, stored in localStorage

### 📊 HUD Elements
- **Orbitron-font score** with teal glow
- **Circular speedometer** — conic-gradient arc that fills dynamically (0–180+ km/h)
- **Distance counter** — auto-formats m → km
- **Level indicator** in orange
- **Health bar** — gradient fill, colour-coded, animated
- **Power-up timers** — slide-in chips with countdown bars
- **Combo notifications** — spring-animated pop-up text

---

## 🧮 Scoring

```
Score per frame = speed × 0.08 × multiplier
Distance (m)   = speed × 0.5 per frame
Level          = floor(score / 500) + 1
Speed          = BASE(4) + level × 0.8
```

---

## 🏗️ Engine Details

- **Canvas 2D API** — everything drawn programmatically, zero images/sprites
- **requestAnimationFrame** loop — smooth 60fps
- **Perspective projection** — `lerp(vanishingPoint, bottomEdge, depthT)` for X, linear for Y
- **Smooth lane changes** — `lerp(currentX, targetX, 0.2)` per frame
- **Particle system** — array of particles with velocity, gravity, life decay
- **Collision detection** — scaled bounding-box check using perspective depth
- **localStorage** — leaderboard persists across sessions

---

*NeonDrive · Pure Canvas · Zero dependencies · Works offline*
