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

## 📸 Screenshots

### Start Screen
![start screen](https://github.com/sourabhv/FlapPyBird/raw/master/screenshots/screenshot1.png)

### In-Game
![in-game](https://github.com/sourabhv/FlapPyBird/raw/master/screenshots/screenshot2.png)

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

## 🌱 Future Work & Enhancements

- ✅ Add AI (NEAT algorithm) to learn to play FlappyBird (popular extension)
- 🟡 High-score system with local persistence
- 🟡 Sound toggle settings and UI improvements
- 🟡 Game restart without reloading
- 🟡 Support for multiplayer or competitive score leaderboard
- 🟡 Difficulty scaling with score

---

## 🚀 Contribution Work (if applicable)

✅ We created a Pull Request that:
- Fixes bug: Pipe overlap rendering at high FPS (PR #xyz)
- Adds a new background skin toggle feature
- Positive feedback received from the maintainer

> _We’ll explain this PR in detail during the viva._

---

## 🤛 FAQs Students Might Ask

1. **Why use `pygame.Rect` instead of pixel-by-pixel collision?**
   - Faster and more optimized collision detection.

2. **How are pipes randomized?**
   - Pipe gap position is randomized within a fixed vertical range using `random.randint()`.

3. **Is frame rate control important?**
   - Yes. A stable `FPS` (usually 30) ensures consistent gameplay experience.

4. **How is gravity implemented?**
   - A velocity variable increases each frame, mimicking acceleration due to gravity.

---

## 📌 References

- [Pygame Documentation](https://www.pygame.org/docs/)
- [Original FlappyBird inspiration](https://en.wikipedia.org/wiki/Flappy_Bird)

