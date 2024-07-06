# Program Documentation & How to make & Information

This document provides an overview and documentation for the Python program `READ.md`. The program is a simple game implemented using the Pygame Zero library. It features two characters, Mario and Luigi, who collect coins while avoiding enemies. The game includes different screens for the home, gameplay, win, and timeout states.

## Table of Contents
1. [Installation](#installation)
2. [Game Overview](#game-overview)
3. [Usage](#usage)
4. [Code Structure](#code-structure)
5. [Functions](#functions)
6. [Constants](#constants)
7. [Objects](#objects)
8. [Conclusion](#conclusion)

## Installation
To run the "Exciting Coin Collectors.py" program, you need to have Python installed on your system. Additionally, you need to install the Pygame Zero library. You can install Pygame Zero using the following command:

```
pip install pgzero
```

Once installed, you can run the program by executing the following command:

```
python test.py
```

## Game Overview
The game implemented in "Exciting Coin Collectors.py" is a simple 2D game where the objective is to collect coins while avoiding enemies. The game consists of several screens:

1. Home Screen: This screen is displayed at the start of the game. It provides instructions and options to start, exit, or switch to fullscreen or normal mode.

2. Gameplay Screen: This screen is displayed when the game starts. It shows the game environment with characters (Mario and Luigi), enemies, coins, and a timer. The characters can be controlled using the arrow keys (Mario) and WASD keys (Luigi).

3. End Screen: This screen is displayed when the game ends. It shows a message and exits the game after a few seconds.

4. Mario Win Screen: This screen is displayed when Mario reaches the win score before Luigi. It shows the scores of both characters.

5. Luigi Win Screen: This screen is displayed when Luigi reaches the win score before Mario. It also shows the scores of both characters.

6. Timeout Screen: This screen is displayed when the timer reaches zero. It shows a message and displays the final scores of both characters.

## Usage
Upon running the program, the game will start with the home screen. The following keyboard commands are available:

- **Space Key**: Pressing the space key on the home screen starts the game.
- **Escape Key**: Pressing the escape key exits the game.
- **f Key**: Pressing the "f" key switches to fullscreen mode.
- **n Key**: Pressing the "n" key switches to normal mode.

During gameplay, the characters can be controlled using the following keys:

- **Arrow Keys**: Control Mario's movement (left, right, up, down).
- **WASD Keys**: Control Luigi's movement (left, right, up, down).

The objective of the game is to collect coins while avoiding enemies. When a character collides with a coin, the score increases, and the coin is randomly relocated. If a character collides with an enemy, the score is reset, and the character is also relocated. The game ends when either character reaches the win score or when the timer reaches zero.

## Code Structure
The `test.py` program follows a structured code organization. It begins with the necessary library imports, followed by the definition of helper functions, event handlers, and drawing functions. The program also defines constants for the game window size and other variables used throughout the game. It concludes with the initialization of objects and the execution of the game using the `pgzrun.go()` function.

## Functions
The program defines several functions to handle various aspects of the game:

- `random_location(actor)`: Sets the position of an actor to a random location within the game window.
- `actor_correct_location(actor)`: Wraps the actor's position around the game window if it goes off-screen.
- `random_enemy_direction()`: Sets the enemy's movement direction randomly and updates its image accordingly.
- `close()`: Quits the game when the window is closed.
- `on_key_down()`: Handles keyboard input events.
- `mushroom_show()`: Shows the mushroom actor at a random location and hides it after 3 seconds.
- `mushroom_hide()`: Hides the mushroom actor off-screen.
- `draw()`: Draws different screens depending on the game status.
- `update()`: Updates the game state, including character movement, collision detection, and score calculation.
- `init()`: Initializes the game by setting initial values for characters, enemies, coins, and other variables.

## Constants
The program defines the following constants:

- `WIDTH`: The width of the game window (1280pixels).
- `HEIGHT`: The height of the game window (720 pixels).

These constants determine the size of the game window and can be adjusted according to your preferences.

## Objects
The program uses several objects to represent different elements in the game:

- `background`: Represents the background image of the game.
- `mario`: Represents the character Mario.
- `luigi`: Represents the character Luigi.
- `enemy`: Represents the enemy character.
- `coin`: Represents the coin that the characters collect.
- `mushroom`: Represents the mushroom actor.

These objects are manipulated and updated throughout the game to create the gameplay experience.

## Conclusion
The "Exciting Coin Collectors.py" program is a simple game implemented using the Pygame Zero library. It features characters, enemies, coins, and various screens to provide an engaging gaming experience. The program demonstrates the usage of Pygame Zero functions, event handling, and basic game logic.

By following the installation instructions and running the program, you can experience the gameplay and explore the code to understand how the various elements of the game are implemented. Feel free to modify and enhance the code to create your own custom game based on the provided structure and functionality.