# 2D-Game-Transformation-Engine🎮


GAME MATRIX — 2D Game Transformation Engine

Engineering Mathematics Mini Project — F3

A Python-based 2D transformation engine that demonstrates how matrix multiplication and transformation composition are used in computer graphics and 2D games.

---

📌 Project Overview

In 2D games, objects such as characters, vehicles, enemies, and other sprites need to be scaled, rotated, and moved on the screen.

This project demonstrates these operations mathematically using 3×3 homogeneous transformation matrices.

The project applies three transformations to a triangle representing a game sprite:

- 🔍 Scaling
- 🔄 Rotation
- 📍 Translation

The transformations are composed as:

[
\boxed{Total = T \times R \times S}
]

The final point is calculated using:

[
\boxed{P' = T \times R \times S \times P}
]

---

🎯 Problem Statement

A sprite or character in a 2D game can:

1. Rotate by an angle θ
2. Scale by a factor s
3. Translate by (tx, ty)

Each operation can be represented using a matrix.

The objective is to compose these transformations and apply them to a triangle, showing the transformation step by step.

---

📐 Mathematical Concepts

This project demonstrates:

- Matrix multiplication
- Homogeneous coordinates
- Transformation matrices
- Transformation composition
- Rotation
- Scaling
- Translation
- Non-commutativity of matrix multiplication
- 2D coordinate transformations

---

🧮 Transformation Matrices

1. Scaling Matrix

For scale factor "s":

[
S =
\begin{bmatrix}
s & 0 & 0\
0 & s & 0\
0 & 0 & 1
\end{bmatrix}
]

2. Rotation Matrix

For rotation angle "θ":

[
R =
\begin{bmatrix}
\cos\theta & -\sin\theta & 0\
\sin\theta & \cos\theta & 0\
0 & 0 & 1
\end{bmatrix}
]

3. Translation Matrix

For translation "(tx, ty)":

[
T =
\begin{bmatrix}
1 & 0 & tx\
0 & 1 & ty\
0 & 0 & 1
\end{bmatrix}
]

---

🔄 Transformation Process

The project performs the transformations in this order:

Original Triangle
       ↓
    Scaling
       ↓
    Rotation
       ↓
   Translation
       ↓
Final Transformed Triangle

Mathematically:

Scaled     = S × P

Rotated    = R × Scaled

Translated = T × Rotated

Therefore:

P' = T × R × S × P

---

🔺 Original Triangle

The project uses a triangle with the following coordinates:

A = (0, 0)
B = (2, 0)
C = (1, 2)

Homogeneous-coordinate representation:

[
P =
\begin{bmatrix}
0 & 2 & 1\
0 & 0 & 2\
1 & 1 & 1
\end{bmatrix}
]

---

🖥️ Features

✅ User Input

The program accepts:

Rotation angle θ
Scale factor s
Translation X (tx)
Translation Y (ty)

Example:

Rotation angle: 45
Scale factor: 2
Translation X: 3
Translation Y: 2

✅ Matrix Display

The program displays:

- Scaling Matrix
- Rotation Matrix
- Translation Matrix
- Total Transformation Matrix

✅ Step-by-Step Calculation

It shows:

Original
   ↓
Scaling
   ↓
Rotation
   ↓
Translation

✅ Final Coordinates

The original and transformed coordinates of points "A", "B", and "C" are displayed.

✅ Transformation Order Comparison

The project compares:

T × R × S

with:

S × R × T

This demonstrates that:

[
T \times R \times S \neq S \times R \times T
]

because matrix multiplication is not commutative.

✅ Static Visualization

The project plots:

- Original triangle
- Scaled triangle
- Rotated triangle
- Final transformed triangle

✅ Animation

An animated visualization shows the triangle gradually undergoing:

Scaling → Rotation → Translation

This makes the mathematical transformation easier to understand visually.

---

🛠️ Technologies Used

Technology| Purpose
Python| Main programming language
NumPy| Matrix calculations
Matplotlib| Graphs and visualization
Matplotlib Animation| Transformation animation
Google Colab| Recommended execution environment

---

📦 Requirements

Install/import the following Python libraries:

import numpy as np
import matplotlib.pyplot as plt
from matplotlib.animation import FuncAnimation
from IPython.display import HTML, display

Google Colab already supports the required libraries in most cases.

---

▶️ How to Run

Option 1 — Google Colab

1. Open Google Colab.
2. Create a new notebook.
3. Copy the project code into a code cell.
4. Run the cell.
5. Enter the transformation values when prompted.
6. View the matrices, calculations, graph, and animation.

Example Input

Enter rotation angle θ (degrees): 45
Enter scale factor s: 2
Enter translation X (tx): 3
Enter translation Y (ty): 2

---

📊 Expected Output

The program produces:

GAME MATRIX
2D GAME TRANSFORMATION ENGINE

INPUT SUMMARY

TRANSFORMATION MATRICES

STEP-BY-STEP CALCULATION

TOTAL TRANSFORMATION

FINAL COORDINATES

TRANSFORMATION ORDER COMPARISON

It then displays a graphical visualization and an animation of the transformed triangle.

---

🎮 Real-World Applications

Transformation matrices are widely used in:

- 🎮 2D Game Development
- 🖥️ Computer Graphics
- 🎨 Animation
- 🤖 Robotics
- 📱 User Interface Graphics
- 🕹️ Sprite Movement
- 🎥 Visual Effects

For example, a game character can be:

Scaled → Rotated → Moved

using exactly the type of mathematical transformations demonstrated in this project.

---

🧠 Key Mathematical Insight

The most important concept demonstrated by this project is that the order of matrix multiplication matters.

For example:

[
T \times R \times S
]

generally produces a different result from:

[
S \times R \times T
]

Therefore, matrix multiplication provides a powerful mathematical way to control the position, size, and orientation of objects in 2D environments.

---

📁 Project Structure

GAME-MATRIX/
│
├── README.md
│
└── game_matrix.py

If using Google Colab:

GAME_MATRIX.ipynb

---

👥 Team

🎮 Team Name: GAME MATRIX

Project: 2D Game Transformation Engine
Project Code: F3
Domain: Engineering Mathematics + 2D Game Graphics

The name GAME MATRIX represents the combination of:

GAME
  +
MATRIX MATHEMATICS

It reflects the project's goal of connecting Engineering Mathematics with gaming through transformation matrices.

---

🏆 Project Objective

The main objective of this project is to demonstrate that mathematical concepts such as matrix multiplication and transformation composition are not only theoretical concepts but also have practical applications in modern technologies such as 2D games and computer graphics.

---

🔮 Future Improvements

The project can be extended with:

- Multiple game sprites
- Interactive controls
- Real-time transformation sliders
- Sprite image loading
- Keyboard-controlled movement
- 2D collision detection
- More complex shapes
- Reflection and shearing transformations
- Interactive game-like interface

---

📜 Conclusion

GAME MATRIX successfully demonstrates how Engineering Mathematics can be applied to a practical 2D gaming scenario.

By representing scaling, rotation, and translation as matrices and combining them through matrix multiplication, a game object can be transformed efficiently and mathematically.

[
\boxed{P' = T \times R \times S \times P}
]

🎮 GAME MATRIX

Where Mathematics Meets Gaming.