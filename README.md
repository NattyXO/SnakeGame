
# Snake Game With C++
This code is a simple implementation of the classic game "Snake" in C++. Let me break down the different parts of the code and provide an explanation:

### Libraries Used:
- `iostream`: For input and output streams.
- `conio.h`: For console input/output.
- `windows.h`: For Windows-specific functionality.

### Variables:
- `gameOver`: Boolean to track if the game is ongoing.
- `width`, `height`: Dimensions of the game area.
- `x`, `y`: Current position of the snake head.
- `fruitX`, `fruitY`: Position of the fruit that the snake eats.
- `score`: Player's score.
- `tailX[100]`, `tailY[100]`: Arrays to store positions of the snake's tail.
- `nTail`: Length of the snake.
- `dir`: Enum to store the direction of the snake.

### Functions:

1. **Setup():**
   - Initializes game variables like position, score, and sets up initial game state.

2. **Draw():**
   - Clears the console and draws the game grid.
   - Renders the snake, fruit, and the game border.
   - Displays the current score.

3. **Input():**
   - Handles keyboard input using `_kbhit()` and `_getch()`.
   - Changes the direction of the snake based on user input ('a', 'd', 'w', 's', 'x' for exit).

4. **Logic():**
   - Manages the game logic.
   - Moves the snake based on its direction.
   - Handles collision detection with the game borders and its own tail.
   - Increases the score when the snake eats the fruit and extends its tail.

5. **Main():**
   - Initializes the game and runs the main game loop until `gameOver` becomes true.
   - Calls `Draw()`, `Input()`, and `Logic()` functions in each iteration.
   - Uses `Sleep(10)` to control the game speed.

### Additional Notes:
- The snake moves continuously in the direction it was last directed until a new direction is given.
- The game ends if the snake collides with the border or itself.
- The player's score increases by 10 points each time the snake eats the fruit.
- The game screen is cleared and redrawn in each iteration to simulate movement.

### Improvements:
- This code could be improved by encapsulating functionalities into classes and using more modern C++ features.
- Adding boundary checking to avoid fruit spawning inside the snake or on the border.
- Implementing a game over screen or message when the game ends.

### Disclaimer:
- Using certain functions like `Sleep()` might make the game less responsive on some systems.
- The code lacks comments and could benefit from better variable naming and explanations for readability and maintainability.

Overall, this is a basic implementation of the Snake game in C++ that could serve as a starting point for more advanced features and improvements.
