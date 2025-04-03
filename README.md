## Coin Rain Adventure

### Overview

**Coin Rain Adventure** is an exciting, fast-paced game built using Pygame where players control a robot to catch falling coins while avoiding falling monsters. The goal of the game is to collect as many coins as possible while avoiding collisions with the monsters. The game ends when the player is hit by a monster.

The game has an intuitive control system, where the player moves left or right to collect coins, and the speed of falling objects increases as the game progresses.

---

### Features

- **Player Control**: Move a robot left and right to catch falling coins.
- **Falling Objects**: Coins and monsters fall from the top of the screen at different speeds.
- **Scoring System**: The player earns points for each coin they catch. The score is displayed at the top left corner.
- **Game Over**: The game ends when the robot collides with a monster.
- **Graphics**: Custom images for the robot, coins, and monsters to enhance the gaming experience.

---

### Controls

- **Left Arrow**: Move the robot left.
- **Right Arrow**: Move the robot right.

---

### Game Flow

1. The game starts with the robot positioned at the bottom of the screen.
2. Coins fall from the top of the screen at a moderate speed. The player must catch the coins to earn points.
3. Monsters also fall from the top, but at a faster rate. If the player’s robot collides with a monster, the game ends.
4. When a coin reaches the bottom of the screen, it respawns at a random position above.
5. The score is incremented each time a coin is collected and is displayed at the top left of the screen.
6. The game continues until the player is hit by a monster.

---

### Installation

To play **Coin Rain Adventure**, you'll need Python and Pygame installed on your computer. Here’s how to get started:

#### Step 1: Install Python

Ensure you have Python installed on your system. You can download it from the official Python website: [Python Downloads](https://www.python.org/downloads/).

#### Step 2: Install Pygame

Once Python is installed, install Pygame using pip:

```bash
pip install pygame
```

#### Step 3: Download the Game Files

Download or clone the repository containing the game files. You’ll need the following files:

- `robot.png`: Image for the player (robot).
- `coin.png`: Image for the falling coins.
- `monster.png`: Image for the falling monsters.
- `game.py`: The main Python file that runs the game.

#### Step 4: Run the Game

After you have all the necessary files, navigate to the folder where your game files are located and run the following command:

```bash
python game.py
```

This will launch the game window, and you can begin playing.

---

### Game Mechanics

#### Player Movement

- The robot is controlled using the **left** and **right arrow keys**.
- The robot cannot move beyond the screen borders.
- The robot will continue to move in the direction of the arrow key until it is pressed again.

#### Falling Objects

- **Coins**: Coins fall from random positions at the top of the screen. The player must catch them to score points.
- **Monsters**: Monsters fall at a faster rate. If the player collides with a monster, the game ends immediately.

#### Collision Detection

- A coin is considered "caught" if the player’s robot collides with it. This is determined based on the robot's position and the coin’s position.
- Similarly, a collision with a monster results in the end of the game.

#### Score

- The score increases by 1 each time the player catches a coin.
- The score is displayed in the top-left corner of the screen.

---

### Customization

You can modify the game by tweaking the following variables:

- **Player Speed**: Adjust the speed at which the player moves by modifying the `player_speed` variable.
- **Coin Speed**: Adjust how fast the coins fall by modifying the coin’s vertical speed in the `update_positions` function.
- **Monster Speed**: Modify the monster’s falling speed to make the game harder by adjusting the vertical speed of monsters.

---

### Future Improvements

Here are some ideas for future updates:

- **Increase Difficulty**: Gradually increase the speed of the falling objects as the player collects more coins.
- **Sound Effects**: Add sound effects when the player collects coins or is hit by a monster.
- **High Score Tracking**: Keep track of high scores to challenge players to beat their best performance.
- **Game Over Screen**: Show a more detailed game over screen with options to restart the game.

---

### License

This game is provided under the [MIT License](LICENSE).
