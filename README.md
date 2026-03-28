# 🐦 Flappy Bird Clone (Pygame)

A high-quality, object-oriented implementation of the classic **Flappy Bird** game built with Python and the **Pygame** library. This project focuses on clean code structure, smooth physics, and scalable game state management.

---

## 🚀 Core Features

* **State Management:** Implements a professional `MenuManager` system to handle transitions between the Home Screen and active Gameplay.
* **Dynamic Physics:** Features realistic bird gravity, jump mechanics, and rotation based on vertical velocity.
* **Adaptive Difficulty:** Game speed and pipe spawn distances increase dynamically as the player's score grows.
* **Procedural Obstacles:** Infinite pipe generation with randomized heights and calibrated gaps for a fair yet challenging experience.
* **Frame-Independent Movement:** Uses **Delta Time (dt)** calculation to ensure consistent movement speeds regardless of the hardware's frame rate.

---

## 🛠️ Project Architecture

The codebase is modularized for better maintainability:

* **`main.py`**: The entry point. Handles the global game loop, event polling, and top-level rendering.
* **`objects.py`**: Contains the core logic for game entities (`Player`, `Pipe`, and a `BaseObject` inheritance class).
* **`menu.py`**: Manages the UI layers, including the animated `HomeScreen` and the main `Game` logic.
* **`config.py`**: A centralized configuration file for constants (screen dimensions, FPS, asset paths) and utility functions like `clamp` and `load_image`.

---

## 📦 Installation & Setup

  **Prerequisites:**
    * Python 3.x
    * Pygame library
    * 
---

## 🎮 How to Play

* **Left Click / UP Arrow:** Flap the wings to gain altitude.
* **Objective:** Fly through the gaps between the green pipes.
* **Game Over:** Hitting a pipe or the ground ends the round. Click the screen to return to the main menu and try again.

---

## 📑 Technical Highlights (for Portfolio)

* **Collision Tuning:** Utilizes the `pygame.Rect.inflate()` method to create smaller, more forgiving hitboxes, improving player satisfaction.
* **Asset Optimization:** Images are processed with `convert_alpha()` for optimized blitting performance.
* **Sprite Animation:** Implements a timer-based animation system for the bird's wings, independent of the game's physics calculations.

---
