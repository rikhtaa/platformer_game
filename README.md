# ⚔️ Code Warrior - Platformer Game

A high-performance 2D platformer game built with **Vanilla JavaScript** and **HTML5 Canvas**. This project serves as a practical implementation of **Intermediate Object-Oriented Programming (OOP)** concepts, focusing on class inheritance, encapsulation, and coordinate-based collision physics.

## 🚀 Features

* **Dynamic Physics Engine:** Implements gravity, velocity, and friction for realistic player movement.
* **Parallax Scrolling:** The world moves relative to the player, creating an expansive level feel.
* **OOP Level Design:** Platforms and Checkpoints are instantiated as objects with their own properties and methods.
* **Collision Detection:** Advanced logic for detecting intersections between the player and environment (platforms and checkpoints).
* **Proportional Scaling:** The game automatically adjusts element sizes based on the viewport height to ensure playability on different screens.

---

## 🛠️ Tech Stack

* **HTML5 Canvas:** For high-performance graphics rendering.
* **CSS3:** Styled with custom properties (variables) and glassmorphism-inspired UI components.
* **JavaScript (ES6+):** Utilizes Classes, `requestAnimationFrame`, and advanced Array methods (`map`, `forEach`, `every`).

---

## 🏗️ Core Architecture (OOP Logic)

The game is structured around three primary classes that manage the game state:

| Class | Responsibility |
| --- | --- |
| **`Player`** | Handles movement, gravity application, and boundary constraints. |
| **`Platform`** | Defines static environmental objects that the player can stand on. |
| **`CheckPoint`** | Manages level progression and "claim" state logic. |

### Physics Logic: Gravity & Collision

The engine uses a constant `gravity` value ($0.5$) applied to the vertical velocity ($\Delta y$) every frame. Collision is calculated by checking if the player's bounding box overlaps with a platform's coordinates:

$$y_{player} + height_{player} + \Delta y \geq y_{platform}$$

---

## 🎮 How to Play

1. **Start:** Click the "Start Game" button on the landing screen.
2. **Move:** Use the **Left/Right Arrow Keys** to navigate.
3. **Jump:** Use **Spacebar** or the **Up Arrow Key**.
4. **Goal:** Reach the yellow checkpoints to progress through the level.

---

## 📦 Project Structure

```text
├── index.html   # Main game structure and UI screens
├── style.css    # Layout, animations, and responsive design
└── script.js    # OOP logic, physics engine, and animation loop

```

---

## 🚦 Getting Started

1. **Clone the repository** to your local machine.
2. **Open `index.html**` in any modern web browser.
3. **Scale the window** to see the proportional sizing logic in action.

---

## 🔮 Future Roadmap

* **Enemies:** Add moving obstacles that reduce player health.
* **Power-ups:** Implement items that increase jump height or speed.
* **Level Editor:** Create a tool to generate `platformPositions` arrays visually.

---

## 👤 Author

**Rekhta**

---

## 📝 License

This project is licensed under the Apache-2.0 License.

