# 🚀 Galactic Interceptor 3D: Elite Edition

> **"The last line of defense between order and total destructioin."**

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![OpenGL](https://img.shields.io/badge/OpenGL-PyOpenGL-green?style=flat&logo=opengl)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 📖 Table of Contents
* [About the Project](#-about-the-project)
* [Lore & Purpose](#-lore--purpose)
* [Key Features](#-key-features)
* [Controls](#-controls)
* [Technical Implementation](#-technical-implementation)
* [Installation & Setup](#-installation--setup)
* [Screenshots](#-screenshots)

---

## 🎮 About the Project
**Galactic Interceptor 3D** is an arcade-style space survival game built from scratch using **Python** and **OpenGL (PyOpenGL)**. 

Unlike standard Unity or Unreal Engine projects, this game constructs its entire world—including the 3D spacecraft models, wireframe enemies, and UI elements—using raw geometric primitives and custom rasterization algorithms. It demonstrates the power of core computer graphics concepts like **Midpoint Algorithms**, **Affine Transformations**, and **Camera Projection math**.

---

## 🌌 Lore & Purpose

### The Story
You step into the cockpit of the **RX-78 "Vanguard,"** the most advanced spacecraft ever built. The galaxy is facing a cataclysmic event known as the **"Starfall"**—rogue geometric entities and fallen stars are collapsing into civilized sectors. Your mission is to hold the line.

### The Mental Flow
This game is designed to induce a state of **"Flow."** * **The Outcome:** The rhythmic destruction of enemies combined with soothing neon visuals transforms anxiety into action.
* **The Reward:** A victory triggers a procedurally drawn "Happy Face" 😊, releasing dopamine and a sense of accomplishment.
* **The Resilience:** A loss triggers a "Sad Face" 😭, evoking empathy and the drive to try again.

---

## ✨ Key Features

### 1. High-Fidelity Modern Spacecraft
A custom 3D model featuring engine thrusters, swept-back wings, and a metallic finish, built entirely from code using `gluCylinder` and `glutSolidCube`.

### 2. Dual Camera System
Toggle between **Cinematic Third-Person** and immersive **First-Person Cockpit** views instantly.

### 3. Adaptive Difficulty
The game evolves with you. 
* **Level 1:** Massive 5-bullet spread shot.
* **Higher Levels:** Firepower focuses, and enemies become faster and more numerous (+2 per level).

### 4. "Ultimate" Cheat Mode
A developer sandbox mode featuring:
* **Invincibility Shield:** A wireframe force field.
* **Spin Attack:** The ship physically rotates 360°.
* **Auto-Aim:** Bullets automatically target the nearest enemy.

### 5. Algorithmic Facial Expressions
Instead of loading images, the game uses the **Midpoint Circle Algorithm** to draw Happy or Sad faces pixel-by-pixel depending on the game outcome.

### 6. Interactive HUD & Menus
A custom 2D Heads-Up Display showing real-time stats, clickable Pause/Exit buttons, and level progression screens.

---

## 🕹 Controls

| Action | Input / Key |
| :--- | :--- |
| **Move Forward/Back** | `W` / `S` |
| **Turn Left/Right** | `A` / `D` |
| **Fire Weapons** | `Left Mouse Click` |
| **Toggle Camera** | `V` |
| **Zoom In/Out** | `Scroll Wheel` or `[` / `]` |
| **Toggle Cheat Mode** | `C` |
| **Pause Game** | Click **PAUSE** Button |
| **Exit Game** | Click **EXIT** Button |

---

## 🛠 Technical Implementation

This project utilizes specific computer graphics algorithms:

* **Midpoint Circle Algorithm:** Used to render the emotive faces on the Win/Loss screens.
* **3D Projection Mapping:** Converts 3D world coordinates to 2D screen space for the HUD overlays.
* **Vector Math:** Used for the "Homing Bullet" logic in Cheat Mode (calculating magnitude and normalized vectors).
* **State Management:** A robust system handling Menu, Play, Level Win, and Game Over states without restarting the application.

---

## ⚙ Installation & Setup

### Prerequisites
* Python 3.6 or higher

### Steps
1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/your-username/galactic-interceptor-3d.git](https://github.com/your-username/galactic-interceptor-3d.git)
    cd galactic-interceptor-3d
    ```

2.  **Install Dependencies**
    You need the `PyOpenGL` library.
    ```bash
    pip install PyOpenGL PyOpenGL_accelerate
    ```
    *(Note: On some Windows systems, if pip fails, you may need to download the pre-built wheels from [Christoph Gohlke's site](https://www.lfd.uci.edu/~gohlke/pythonlibs/#pyopengl)).*

3.  **Run the Game**
    ```bash
    python main.py
    ```

---

## 📸 Screenshots

*(Add screenshots of your game here)*

| First Person View | Third Person View |
| :---: | :---: |
| ![FPS View](placeholder-image-1.png) | ![TPS View](placeholder-image-2.png) |

| Cheat Mode (Shield) | Game Over (Sad Face) |
| :---: | :---: |
| ![Cheat Mode](placeholder-image-3.png) | ![Sad Face](placeholder-image-4.png) |

---

## 📜 License
This project is open-source and available for educational purposes.

**Author:** [Shafin Mahamud]  
**Course:** CSE423 - Computer Graphics
