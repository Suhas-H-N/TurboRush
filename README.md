# 🚗 NeonDrive — Modern Arcade Racing Game

<div align="center">

### High-Speed Perspective Racing Built with Pure HTML5 Canvas

*A visually immersive arcade racing experience featuring procedural graphics, dynamic gameplay, and zero external dependencies.*

**HTML5 • CSS3 • JavaScript • Canvas API • Local Storage**

</div>

---

## 📖 Overview

**NeonDrive** is a modern browser-based arcade racing game inspired by classic endless highway racers. Built entirely with the **HTML5 Canvas API**, the game recreates a fast-paced pseudo-3D driving experience using procedural rendering techniques—without relying on game engines, images, or third-party libraries.

Players navigate through high-speed traffic, collect powerful upgrades, maintain combo streaks, and compete for the highest score while the game continuously increases in difficulty.

The project demonstrates advanced front-end development concepts including:

- Real-time Canvas rendering
- Procedural graphics
- Game loop architecture
- Collision detection
- Particle systems
- Responsive controls
- Local storage persistence
- Performance-optimized animations

---

# ✨ Highlights

- 🎨 Fully procedural graphics (No images or sprites)
- 🏎️ Pseudo-3D perspective highway
- 🌃 Dynamic neon city environment
- ⭐ Animated star field
- 💥 Particle-based explosion system
- 🚘 Smooth lane transition physics
- ⚡ Multiple power-up mechanics
- ❤️ Health system with visual feedback
- 📈 Progressive difficulty scaling
- 🏆 Persistent leaderboard
- 📱 Mobile touch controls
- 🌙 Modern cyberpunk-inspired UI
- ⚙️ Zero external libraries
- 🌐 Works completely offline

---

# 🚀 Quick Start

Simply open the project in any modern web browser.

```text
Double-click index.html
```

No installation required.

No build process.

No package manager.

No internet connection required.

---

# 🎮 Controls

| Key | Action |
|------|---------|
| ← | Move Left |
| → | Move Right |
| A | Move Left |
| D | Move Right |
| P | Pause / Resume |
| Esc | Pause Menu |
| Touch Buttons | Mobile Steering |
| Swipe Left | Change Lane |
| Swipe Right | Change Lane |

---

# 📂 Project Structure

```text
NeonDrive/
│
├── index.html
│   ├── Main Game Screen
│   ├── Title Screen
│   ├── Game Over Screen
│   ├── Leaderboard
│   └── How To Play
│
├── style.css
│   ├── Dark Neon Theme
│   ├── Responsive Layout
│   ├── HUD Styling
│   ├── UI Animations
│   └── Screen Transitions
│
├── game.js
│   ├── Game Engine
│   ├── Rendering System
│   ├── Physics
│   ├── Collision Detection
│   ├── Power-Ups
│   ├── Particle System
│   ├── Leaderboard Logic
│   └── Input Handling
│
└── README.md
```

---

# 🎨 Visual Experience

NeonDrive delivers a modern cyberpunk-inspired visual experience completely generated using the Canvas API.

## Dynamic Road Rendering

- Perspective highway rendering
- Animated lane markings
- Infinite scrolling road
- Vanishing-point projection
- Smooth road movement

---

## Procedural City

The background cityscape is generated dynamically and includes:

- Multi-layer skyline
- Randomized building heights
- Illuminated windows
- Parallax scrolling
- Atmospheric depth

---

## Animated Sky

- Procedural stars
- Twinkling animation
- Smooth opacity transitions
- Infinite night environment

---

## Vehicle Rendering

Every vehicle is drawn directly using Canvas.

Features include:

- Gradient body paint
- Windshield reflections
- Wheels
- Brake lights
- Headlights
- Perspective scaling

No sprite sheets are used.

---

## Visual Effects

The game includes numerous particle and lighting effects:

- Collision explosions
- Speed particles
- Boost trails
- Collection bursts
- Neon glow rendering
- Motion feedback

---

# 🏎 Gameplay Features

## Five-Lane Racing

Players drive across five lanes using smooth interpolated lane transitions.

---

## Progressive Difficulty

Game difficulty scales automatically by increasing:

- Vehicle speed
- Traffic density
- Spawn frequency
- Score multiplier opportunities

Every 500 points advances the player to the next level.

---

## Health System

Players begin with:

❤️❤️❤️

Three shield points.

The health bar dynamically changes color:

- 🟢 Safe
- 🟡 Warning
- 🔴 Critical

---

## Combo System

Successfully avoiding traffic consecutively builds combo chains.

Combo Levels

- 5 Dodges
- 10 Dodges
- 15 Dodges
- 20+ Dodges

Higher combos increase score multipliers.

---

# ⚡ Power-Ups

| Power-Up | Description | Duration |
|-----------|-------------|----------|
| 🛡 Shield | Restore one health point (Maximum 3) | Instant |
| ⚡ Boost | Double score multiplier | 5 Seconds |
| 🧲 Magnet | Automatically attracts nearby power-ups | 3 Seconds |
| ⭐ Star | Complete collision immunity | 4 Seconds |

---

# 🏆 Game Screens

### Title Screen

- Animated road preview
- Live traffic
- Best score display
- Menu navigation

---

### Gameplay Screen

Includes a fully interactive HUD:

- Live score
- Circular speedometer
- Distance tracker
- Current level
- Health indicator
- Active power-up timers
- Combo notifications

---

### Game Over

Displays:

- Final Score
- Distance Covered
- Highest Speed
- Maximum Combo
- Highest Level
- Best Score Indicator

---

### Leaderboard

Stores the Top 20 scores locally using browser storage.

Features:

- Gold
- Silver
- Bronze medals

Persistent across browser sessions.

---

# 📊 HUD Components

The HUD includes:

- Neon Orbitron score display
- Animated speedometer
- Distance counter
- Level tracker
- Dynamic health bar
- Power-up countdowns
- Combo notifications
- Visual score multiplier

---

# 🧮 Scoring System

```text
Score      = Speed × 0.08 × Multiplier

Distance   = Speed × 0.5

Level      = floor(Score / 500) + 1

Speed      = Base Speed + (Level × 0.8)
```

---

# ⚙ Technical Implementation

## Rendering

- HTML5 Canvas 2D API
- requestAnimationFrame Game Loop
- Perspective Projection
- Dynamic Scaling
- Layered Rendering Pipeline

---

## Physics

- Smooth lane interpolation
- Velocity updates
- Depth scaling
- Collision bounds
- Spawn management

---

## Effects

- Particle engine
- Glow rendering
- Animation timers
- Procedural generation
- Motion interpolation

---

## Storage

Browser Local Storage is used for:

- High Scores
- Leaderboard
- Best Score

No backend required.

---

# 💻 Technologies Used

- HTML5
- CSS3
- JavaScript (ES6)
- HTML5 Canvas API
- Local Storage

---

# 🌟 Key Highlights

- Pure Canvas Rendering
- No Images
- No Sprite Sheets
- No Game Engine
- No Frameworks
- No Dependencies
- Offline Compatible
- Responsive Design
- Mobile Friendly
- Lightweight
- High Performance

---

# 🎯 Future Improvements

- Sound Effects
- Background Music
- Additional Vehicle Types
- Weather Effects
- Boss Challenges
- Daily Missions
- Online Leaderboard
- Multiplayer Mode
- Garage & Vehicle Customization
- Achievement System
- Controller Support
- Cloud Save

---

# 📄 License

This project is intended for educational purposes and portfolio demonstration.

Feel free to explore, modify, and learn from the source code.

---

<div align="center">

## 🚗 NeonDrive

**Built with HTML5 Canvas • JavaScript • CSS3**

*A modern arcade racing experience showcasing procedural graphics, real-time rendering, and game development techniques using pure web technologies.*

⭐ If you enjoyed this project, consider starring the repository!

</div>
