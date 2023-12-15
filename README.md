### Snake Game 
using C++ console output.
### Header Files
- `#include <iostream>`: Standard input-output stream.
- `#include <conio.h>`: Provides console input/output functions.
- `#include <windows.h>`: Includes functions for console manipulation and sleeping.

### Global Variables
- `gameOver`: Flag to control the game loop.
- `width` and `height`: Dimensions of the game board.
- `x` and `y`: Snake's current position.
- `fruitX` and `fruitY`: Position of the fruit for the snake to eat.
- `score`: Player's score.
- `tailX` and `tailY`: Arrays to store the tail positions of the snake.
- `nTail`: Length of the snake's tail.
- `enum eDirecton`: Enumerated type for defining directions.

### Functions
- `Setup()`: Initializes game variables, positions, and randomizes the fruit's position.
- `Draw()`: Draws the game board, snake, fruit, and displays score.
- `Input()`: Handles user input to change the snake's direction.
- `Logic()`: Manages the game logic including snake movement, collision detection, and fruit eating.

### Main Function
- `main()`: Sets up the game, runs the game loop, and controls the game's flow.

### Game Logic
- The snake moves through user input ('a', 'd', 'w', 's') and cannot move backward.
- The snake grows in length when it eats the fruit, increasing the score.
- The game ends if the snake collides with the boundary or itself (`gameOver` is set to true).

### Remarks
- The game loop continuously updates the screen, takes input, and processes the logic.
- The snake's position, tail, and fruit position determine the game's state and progression.
- Written by 'NattyXO' with credits to 'NVitanovic' from a YouTube tutorial.
- The source code is available on GitHub under the repository 'NattyXO' for further reference and explanations.

### Potential Enhancements
- Implementing levels or increasing difficulty over time.
- Adding sound effects or graphical improvements.
- Enhancing collision detection or adding power-ups.

This game is a basic rendition of Snake, illustrating fundamental concepts of game development in C++. Feel free to modify and expand upon it for further learning or entertainment purposes!