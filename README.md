# 👾 Alien Invasion (Python Crash Course – Chapter 12)

This is a classic **2D arcade-style game** built with [Pygame](https://www.pygame.org), based on Chapter 12 of *Python Crash Course* by Eric Matthes.

In *Alien Invasion*, the player controls a spaceship that moves horizontally across the bottom of the screen and fires bullets upward to destroy an invading alien fleet. The goal is to clear wave after wave of aliens, manage limited lives, and push your **high score** higher with each run.

---

## 🎮 Project Overview

This version goes beyond the early single-alien prototype and implements a full gameplay loop:

- **Full Alien Fleet**: A fleet of aliens is generated and moves across the screen, dropping down a row when it hits an edge.
- **Bullet Management**: The player can fire bullets with the spacebar, with a limit on the number of bullets on screen at once.
- **Lives System**: The player has a limited number of ships. Colliding with an alien or letting aliens reach the bottom costs a life.
- **Scoreboard & HUD**:
  - Current score  
  - High score (persisted between sessions)  
  - Current level  
  - Remaining ships represented by ship icons
- **Progressive Difficulty**: After each wave, game speed and alien point values scale up to increase the challenge.
- **Game Flow & UI**:
  - Game starts in an inactive state with a **Play** button.
  - Press **P** or click **Play** to start.
  - When you lose all ships, a centered **GAME OVER** box appears.
  - A **Play Again** button lets you immediately restart a new run.

Overall, this project shows how small iterative changes can grow into a complete, replayable game experience.

---

## 🧠 Skills & Concepts Demonstrated

- **Pygame fundamentals**
  - Game loop and frame rate management
  - Screen updates, drawing sprites, and handling collisions
- **Object-Oriented Design**
  - Classes for `Ship`, `Alien`, `Bullet`, `Settings`, `GameStats`, `Scoreboard`, and `Button`
  - Clear separation of responsibilities across modules
- **Event-Driven Programming**
  - Handling keyboard input (movement, shooting, quitting, starting)
  - Handling mouse events (Play / Play Again button clicks)
- **State & Data Management**
  - Tracking score, high score, level, and remaining ships via `GameStats`
  - Persisting the **high score** in `high_score.json` with `json` I/O
- **Game Balancing & Tuning**
  - Dynamic difficulty scaling (ship, bullet, and alien speeds)
  - Alien point scaling across levels
- **User Interface Elements**
  - On-screen scoreboard and ship icons using Pygame fonts and sprite groups
  - Overlay **Game Over** message and restart button for a clean user experience
- **Clean Code Structure**
  - Modularized settings and game logic
  - Readable, maintainable structure suitable for extension

---

## 🚀 Development Progress

**Completed Milestones**

1. Basic ship rendering and smooth left/right movement  
2. Bullet creation, movement, and cleanup  
3. Alien sprite class and fleet generation  
4. Fleet movement logic (horizontal movement + drop on edge)  
5. Bullet–alien collision detection and alien removal  
6. Level progression with increasing speed and alien point values  
7. Life system with limited ships and game-over condition  
8. Scoreboard with current score, level, remaining ships, and high score  
9. High score persistence to `high_score.json`  
10. Start screen with Play button and **GAME OVER** overlay plus **Play Again** button

**Planned Enhancements**

- Sound effects for firing, collisions, and game events  
- Additional alien and ship graphics for visual variety  
- Pause functionality and/or in-game options menu  
- Difficulty modes (e.g., Easy / Normal / Hard)  
- Power-ups or special bullet types

---

## 📂 File Structure

```text
Alien_Invasion/
├── alien_invasion.py      # Main game loop and high-level control flow
├── settings.py            # Static & dynamic game configuration, speed/score scaling
├── ship.py                # Player ship class (movement & drawing)
├── bullet.py              # Bullet class (position, movement, rendering)
├── alien.py               # Alien class (movement, edge detection)
├── game_stats.py          # Tracks score, high score, ships left, and level
├── scoreboard.py          # Renders HUD: score, high score, level, ship icons
├── button.py              # Generic clickable button (Play / Play Again)
├── high_score.json        # Persists the all-time high score between sessions
├── images/                # Sprite assets (aliens, ships, etc.)
├── img.png                # Screenshot or reference image from the game
├── LICENSE                # MIT License
├── main.py                # PyCharm stub (not used to run the game)
└── README.md              # Project documentation (this file)
```

> Note: The game is launched via `alien_invasion.py`, not `main.py`.

---

## ▶️ How to Run

1. **Install Pygame**

   ```bash
   pip install pygame
   ```

2. **Run the Game**

   From the project directory:

   ```bash
   python alien_invasion.py
   ```

3. **Controls**

   - **Left / Right Arrow Keys** – Move the ship  
   - **Spacebar** – Fire bullets  
   - **P** – Start the game (in addition to clicking Play)  
   - **Q** – Quit the game  

   When the game ends:
   - A **GAME OVER** message appears.
   - Click **Play Again** to restart a fresh run.

---

## 💻 Requirements

- Python 3.10+  
- Pygame 2.0+  
- Desktop OS: macOS, Windows, or Linux

---

## 📜 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

---

## 🔗 Related Projects

- [Learning Log](https://github.com/E-Conners-Lab/The_Learning_log) – A full Django web app built from Chapters 18–20 of *Python Crash Course*  
- [Python Crash Course Projects](https://github.com/ECbball333/Python-Crash-Course-Project) – Hands-on exercises and projects from earlier chapters  

---

## 📣 Developer Note

This game is part of my ongoing journey expanding from network engineering into deeper Python and software development work. Building *Alien Invasion* from the ground up — and extending it with UI elements, progression, state persistence, and a full game loop — has strengthened my understanding of:

- Object-oriented design
- Event-driven programming
- Working with third-party libraries like Pygame
- Structuring small projects so they are easy to extend and maintain

More enhancements will be added over time as I continue iterating on both my Python skills and this project.
