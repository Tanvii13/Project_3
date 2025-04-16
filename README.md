# Project_3

### Group Name : Titans
### Name : Tanvi Nakum
### Student ID : 202401262
### Project Name : FlapPyBird  
### Github Repository : https://github.com/sourabhv/FlapPyBird/tree/master

# FlapPyBird - Open Source Project Presentation

## 🐤 About the Project

**FlapPyBird** is a Python implementation of the popular mobile game **Flappy Bird**, using the **Pygame** library. Originally developed by [sourabhv](https://github.com/sourabhv/FlapPyBird), it aims to recreate the side-scrolling, single-button gameplay where the player controls a bird trying to fly between sets of pipes.

- **Project Repository (Original)**: [https://github.com/sourabhv/FlapPyBird](https://github.com/sourabhv/FlapPyBird)
- **Forked Repository (Our Work)**: *[insert your forked repo link here]*

## 🎯 Objectives of the Game

- Simulate gravity-driven vertical motion for a bird.
- Generate obstacles (pipes) at regular intervals with gaps at random heights.
- Create continuous side-scrolling gameplay with collision detection.
- Keep track of score based on how many pipes the bird passes.

---

## 🛠️ Local Setup Instructions

### Prerequisites

- Python 3.x
- pip
- pygame (`pip install pygame`)

### Steps

```bash
# Clone the forked repository
git clone https://github.com/yourusername/FlapPyBird.git
cd FlapPyBird

# Install dependencies
pip install -r requirements.txt

# Run the game
python flappybird.py
```

> Note: The game runs in a GUI window. Press the **Spacebar** to make the bird flap.

---

## 🧠 Basic Working of the Game

### Core Mechanics

- The bird automatically falls due to gravity.
- Pressing space makes the bird flap upward.
- Pipes move from right to left.
- The game ends if the bird hits the ground or a pipe.

### Main Files

| File            | Purpose                                   |
|-----------------|-------------------------------------------|
| `flappybird.py` | Main game loop, event handling, rendering |
| `sprites/`      | Game assets (bird, pipes, background)     |
| `README.md`     | Project documentation                     |

---

## 🧱 Data Structures Used

| Data Structure | Usage                                                                 |
|----------------|-----------------------------------------------------------------------|
| **Dictionary** | For configuration settings and storing game state variables          |
| **Lists**      | Managing dynamic game elements like moving pipes                     |
| **Tuples**     | For coordinates and image positioning                                |
| **Rect**       | Pygame’s `Rect` objects used for hitbox and collision calculations   |

---

## ⚙️ How Things Are Modeled

| Component        | Modeled As                                      |
|------------------|--------------------------------------------------|
| Bird             | Sprite object with position, velocity, and image |
| Pipes            | List of dictionaries with x, y, height           |
| Ground & Scenery | Static background image, scrolling floor surface |
| Game Physics     | Velocity, gravity, and acceleration variables    |
| Score            | Integer counter incremented per pipe passed      |

---

## 📌 References

- [Pygame Documentation](https://www.pygame.org/docs/)
- [Original FlappyBird inspiration](https://en.wikipedia.org/wiki/Flappy_Bird)

