<div align="center">

```
 ___  ____  ____  ___  ____     __  __ _  _  __  ____  ____  ____  ___
/ __)(  _ \( ___)/ __)( ___)   (  )(  ( \\ \/ /(  __)(_  _)(  __)/ __)
\__ \ ) __/ )__)( (__  )__)     )( /    / \  /  ) _)   )(   ) _) \__ \
(___/(__)  (____)\___)(____) __(__)\_)__)  \/  (____)  (__) (____)(___/
```

### 👾 A Classic Arcade Shooter — Built with Python & Pygame

<br/>

<p>
  <img src="https://img.shields.io/badge/Python-85.4%25-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Java-14.6%25-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Pygame-Game_Engine-00B140?style=for-the-badge&logo=python&logoColor=white"/>
</p>

<br/>

```
 ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
 ░  👾  👾  👾  👾  👾  👾  👾  ░
 ░  👾  👾  👾  👾  👾  👾  👾  ░
 ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
               |  |
              🚀
```

> *Defend the galaxy. Beat the boss. Don't let them reach you.*

---

</div>

## ✦ About

**Space Invader** is a fully playable recreation of the classic arcade game, built from scratch in Python using Pygame. It features smooth player movement, bullet mechanics, enemy waves, a powerful **boss enemy** that spawns every 500 points, a scrolling starfield background, full sound effects, and a persistent **high score system**.

A bonus `CoinChange.java` dynamic programming solution is also included in the repo — a nod to the DSA side of development.

---

## ✦ Features

| Feature | Details |
|---|---|
| 🚀 **Player Movement** | Smooth left/right movement with boundary clamping |
| 🔫 **Bullet System** | Fire with `SPACE` — single active bullet with ready/fire state machine |
| 👾 **Enemy Waves** | Enemies spawn randomly, drift downward, and reset on hit or escape |
| 💀 **Boss Battles** | A boss spawns every 500 points — takes 5 hits, moves side to side, gets harder each round |
| 💥 **Collision Detection** | Distance-based `math.hypot` collision for both enemy and boss |
| 🌟 **Scrolling Starfield** | 100 animated stars drift downward for an immersive space feel |
| 🔊 **Sound Effects** | Explosion, winning fanfare, and looping background music |
| 🏆 **High Score** | Persistent high score saved to and loaded from `highscore.txt` |
| 🖥️ **Start & Win Screens** | Press ENTER to start; a win screen triggers on a new high score |

---

## ✦ Gameplay

```
Controls:
  ←  →       Move your spaceship left and right
  SPACE       Fire a bullet
  ENTER       Start the game from the title screen
```

### Scoring

| Event | Points |
|---|---|
| Destroy an enemy | +10 pts |
| Defeat the boss | +50 pts |
| Boss spawns every | 500 pts |
| Boss health scales | ×2 each appearance |

### Game Over

The game ends when an enemy reaches your spaceship's Y position. Your score is saved automatically — beat it next run!

---

## ✦ Tech Stack

| Technology | Role |
|---|---|
| Python 3 | Core game logic |
| Pygame | Rendering, input, audio, display |
| `math.hypot` | Collision distance calculations |
| `random` | Enemy & boss spawn positions |
| File I/O | High score persistence (`highscore.txt`) |

---

## ✦ Project Structure

```
Space-Invader/
├── Space Invader.py     # Main game — all logic, loop, rendering
├── spaceship.png        # Player sprite (64×64)
├── enemy.png            # Enemy sprite (32×32)
├── boss.png             # Boss sprite (128×128)
├── bullet.png           # Bullet sprite (32×32)
├── ufo.png              # Window icon
├── background.mp3       # Looping background music
├── explosion.mp3        # Hit / death sound effect
├── winning.mp3          # New high score fanfare
├── highscore.txt        # Persistent high score storage
└── CoinChange.java      # Bonus: Dynamic Programming — Coin Change problem
```

---

## ✦ Getting Started

### Prerequisites

- [Python 3.7+](https://www.python.org/downloads/)
- [Pygame](https://www.pygame.org/)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Kris-Zar/Space-Invader.git
cd Space-Invader

# 2. Install Pygame
pip install pygame

# 3. Run the game
python "Space Invader.py"
```

> ⚠️ All asset files (`spaceship.png`, `enemy.png`, `background.mp3`, etc.) must be in the **same directory** as the script.

---

## ✦ Boss System

The boss is no ordinary enemy. Here's how it works:

- **Spawns** when your score hits a multiple of 500 (e.g. 500, 1000, 1500…)
- **Moves** horizontally across the screen, bouncing off the edges
- **Takes 5 hits** to defeat — each hit deals 10 damage to 50 HP
- **Gets harder** — each time you defeat the boss, its health pool doubles (`bossDamagemultiplier × 2`)
- **Worth 50 points** on defeat

---

## ✦ Bonus — CoinChange.java

The repo also includes a Java solution to the classic **Coin Change** dynamic programming problem (LeetCode #322). It finds the minimum number of coins needed to make up a given amount.

```bash
# Compile and run
javac CoinChange.java
java CoinChange
```

---

## ✦ Roadmap

- [ ] Multiple simultaneous enemies
- [ ] Enemy bullet fire (they shoot back!)
- [ ] Lives / health system
- [ ] Difficulty levels (Easy / Normal / Hard)
- [ ] Pygame sprite groups refactor
- [ ] Leaderboard with player names

---

## ✦ License

Open source — feel free to fork, learn from it, and build upon it. Attribution appreciated.

---

<div align="center">

<br/>

Built with 🐍 + 🎮 by **Parth Saxena**

<br/>

```
INSERT COIN TO CONTINUE . . .
```

<br/>

⭐ *If this brought back arcade memories, leave a star!*

</div>
