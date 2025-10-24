# ASCII Slot Machine Game (C++)

This project is a C++ console-based animated slot machine game built using Object-Oriented Programming (OOP) concepts and ANSI color-coded ASCII graphics.  
It demonstrates structured class design, inheritance, polymorphism, custom exception handling, and basic animation logic using sleep and screen refresh techniques.

---

## Features

- Slot machine logic that randomly generates three numbers.
- Animated display using ASCII blocks (`█`) with ANSI color codes.
- Object-oriented architecture:
  - Classes for rendering, object maintenance, and game logic.
  - Inheritance and virtual functions for modular design.
- Custom exception handling to manage invalid number generation.
- Frame-by-frame rendering using timed screen updates (`usleep`, `sleep`).
- Displays WIN or LOSE based on the slot results.

---

## Tech Stack

- **Language:** C++  
- **Libraries Used:**
  - `<iostream>`, `<string>`
  - `<cstdlib>`, `<ctime>` for randomness
  - `<unistd.h>` for timing (sleep/usleep)

---

## Concept Overview

The game simulates a slot machine:
1. Displays an ASCII-based animated "HI" intro and frame layout.
2. Generates random numbers (0–9) for three slots.
3. Renders the slot results visually in colored ASCII.
4. If all three numbers match → WIN, else → LOSE.

Each visual component (numbers, frame, message, etc.) is drawn by mapping coordinates on a 2D character grid (`p[dim1][dim2]`).

---

## How to Run

### Prerequisites
Ensure you have:
- A Linux or macOS terminal (supports ANSI escape codes)
- A C++ compiler (g++)

### Compile the Code

```bash
g++ -o slot_game main.cpp

### Run the code
./slot_game

