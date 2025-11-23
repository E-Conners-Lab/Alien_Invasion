# 👾 Alien Invasion (Python Crash Course – Chapter 12)

This is a classic **2D arcade-style game** project built using [Pygame](https://www.pygame.org/), based on Chapter 12 of *Python Crash Course* by Eric Matthes.

In *Alien Invasion*, the player controls a spaceship that moves horizontally across the bottom of the screen and shoots bullets upward to destroy incoming aliens. The goal is to clear waves of alien fleets before they reach the bottom or collide with your ship.

---

## 🎮 Project Overview

This version of the game demonstrates key concepts in object-oriented programming and game logic:

- **Ship Movement**: Smooth left-right navigation using continuous keypress detection.
- **Bullet Firing**: Spacebar triggers bullets that travel upward.
- **Alien Sprite**: A single alien is currently displayed and tracked.
- **Game Loop**: Real-time rendering and collision detection structure are in place.
- **Settings Management**: Game settings are stored in a separate module for easy tweaking.
- **Game Statistics**: A game stats object to track ship limits and end conditions.

---

## 🧱 Skills & Concepts Demonstrated

- Pygame setup and game loop mechanics
- Class-based architecture (e.g., `Ship`, `Alien`, `Bullet`, `GameStats`)
- Handling user input and events
- Collision detection and object cleanup
- Modular code design using settings and helper classes
- Image loading and sprite rendering
- Tracking player state (score, remaining ships)

---

## 🚧 Next Steps in Development

The following enhancements are part of the roadmap as outlined in the book:

1. **Add a single alien** – ✅ *(Complete)*
2. **Create a fleet of aliens** - ✅ *(Complete)*
3. **Make the fleet move sideways and drop down** - ✅ *(Complete)*
4. **Detect bullet-alien collisions and remove aliens** - ✅ *(Complete)*
5. **Limit ships and end game on collision or missed invaders** - ✅ *(Complete)*

These incremental improvements build problem-solving skills while providing deeper insight into game development workflows.

---

## 📁 File Structure

```
Alien_Invasion/
├── alien_invasion.py      # Main game loop
├── settings.py            # Game configuration
├── ship.py                # Ship class
├── bullet.py              # Bullet class
├── alien.py               # Alien class
├── game_stats.py          # Player state tracker
├── images/                # Alien and ship sprites
├── LICENSE
└── README.md
```

---

## ▶️ How to Run

1. **Install Pygame**:
   ```bash
   pip install pygame
   ```

2. **Run the Game**:
   ```bash
   python alien_invasion.py
   ```

---

## 🛠 Requirements

- Python 3.10+
- Pygame 2.0+
- Works on macOS, Windows, and Linux

---

## 📜 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## 🔗 Related Projects

- [Learning Log](https://github.com/E-Conners-Lab/The_Learning_log) – A full Django web app built from Chapters 18–20
- [Python Crash Course Projects](https://github.com/ECbball333/Python-Crash-Course-Project) – Hands-on code from Chapters 1–17

---

## 📣 Developer Note

This project represents a key part of my learning journey in software development. While I’m a network engineer by trade, building this game from scratch has deepened my appreciation for the structure and creativity of application development. Stay tuned — more game logic, UI elements, and features are coming soon!
