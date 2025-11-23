# 👾 Alien Invasion – Python Game Project

This is a **2D space shooter game** built as part of **Chapter 12** from *Python Crash Course* by Eric Matthes. The player controls a ship at the bottom of the screen, firing bullets to destroy a descending fleet of aliens.

The game is built using the **Pygame** library and introduces core game development principles such as:

- Screen drawing and updating
- Event loops and user input handling
- Collision detection
- Game settings and behaviors encapsulated in classes

---

## 🎮 Game Features

- Player-controlled spaceship using arrow keys
- Alien fleet movement that adapts to screen edges
- Bullets fired by the player to destroy aliens
- Collision detection between bullets and aliens
- Automatic screen updates with `pygame.time.Clock()`

---

## 📂 Project Structure

```
Alien_Invasion/
│
├── alien_invasion.py         # Main game loop and logic
├── README.md                 # Project documentation
└── .venv/                    # Virtual environment (excluded in .gitignore)
```

---

## 🧠 Skills Demonstrated

This project covers the foundations of game development and object-oriented programming in Python:

### 🔹 Object-Oriented Programming
- Classes and instances (`Ship`, `Alien`, `Bullet`, `Settings`)
- Encapsulation of logic in methods
- Game loop structure and management

### 🔹 Pygame Fundamentals
- Drawing images and shapes
- Detecting keypresses (`KEYDOWN`, `KEYUP`)
- Grouping sprites and managing collisions
- Updating screen efficiently with `pygame.display.flip()`

---

## 🚀 Getting Started

### 🔧 Requirements
Ensure you have Python and `pygame` installed:

```bash
pip install pygame
```

### ▶️ Run the game

```bash
python alien_invasion.py
```

Use **arrow keys** to move the ship, and **spacebar** to fire bullets.

---

## 📖 What’s Next?

This project is just the beginning. Coming up in later chapters of *Python Crash Course*:

- Adding scoring and game stats
- Increasing difficulty levels
- Adding play buttons and menus
- Saving high scores
- More interactive game elements

This marks a key milestone in my full-stack learning journey, balancing backend, frontend, and now game logic. It’s exciting to see how Python can power everything from automation and web apps to games.

---

## 🧠 Broader Learning Goals

While I’m a **network engineer** at heart, this project reinforces the creative potential of software development. Once I complete the final game chapters, I’ll return to applying Python to:

- Network automation with APIs (REST/NETCONF)
- Building interactive dashboards
- Exploring LLMs to help manage and troubleshoot networks

---

## 📜 License

This project is open-sourced under the [MIT License](./LICENSE).
