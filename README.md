# Interactive Hand-Controlled Ball Game

This project is an interactive game that combines **computer vision** with **physics-based simulation**. The goal is to create a real‑time system where the user’s hand position (captured via webcam) is mapped to control an in‑game paddle. A ball moves around the screen under the influence of gravity, bouncing off all edges except the bottom. The user must prevent the ball from falling off the screen by moving the paddle with their hand.

## Overview

- **Computer Vision:**  
    Uses OpenCV (and optionally MediaPipe Hands) to detect and track the user’s hand in real time, mapping its position to control the in‑game platform.

- **Simulation and Modeling:**  
    Implements ball motion and collision dynamics using Newtonian mechanics. The simulation assumes fully elastic collisions with no friction, ensuring realistic ball behavior.

- **Game Mechanics:**  
    - Gravity‑driven ball motion.
    - Collision detection between the ball, walls, and the user-controlled paddle.
    - Score tracking, game‑over conditions, and difficulty settings (including potential multiple‑ball scenarios).

## Features

- **Real-Time Hand Tracking:**  
    Accurate and responsive hand detection using OpenCV and contour detection/MediaPipe models.

- **Physics-Based Simulation:**  
    Realistic ball dynamics based on Newtonian physics, with collision and rebound mechanics.

- **Interactive Gameplay:**  
    Players must use their hand to keep the ball in play, with increasing difficulty levels and score tracking.

- **Modular Code Structure:**  
    Clearly separated modules for computer vision, simulation, and game mechanics to simplify future enhancements and testing.

## Installation

1. **Clone the Repository:**

        ```bash
        git clone https://github.com/yourusername/interactive-hand-ball-game.git
        cd interactive-hand-ball-game

2. **Set Up the Environment:**
    - Create a virtual environment (optional but recommended):
       ```bash
        python -m venv venv
        source venv/bin/activate  # On Windows, use venv\Scripts\activate
- Install the required packages:
    ```bash
    pip install -r requirements.txt
- Requirements may include:
    - ```opencv-python```
    - ```mediapipe``` (if using MediaPipe for hand tracking)
    - ```numpy```
    - ```pygame``` (or any other game library if applicable)
3. **Run the Game:**
    ```bash
    python main.py
