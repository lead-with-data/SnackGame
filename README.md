# Snack Game

## Demo
<!-- Add your video demo here -->


## Architecture & Object-Oriented Programming (OOP)
This project is built using Python's `turtle` graphics library and strictly follows Object-Oriented Programming (OOP) principles to keep the codebase modular, maintainable, and scalable. 

The game is divided into specific classes, each handling its own responsibilities:

* **`Snack` (in `snack.py`)**: 
  * Manages the snake's body segments and movement mechanics.
  * Handles directional changes (`up`, `down`, `left`, `right`) ensuring the snake cannot reverse directly into itself.
  * Controls the growth of the snake (`size()` method) when food is consumed.
  * Manages the snake's reset behavior when a game over occurs.
* **`Food` (in `food.py`)**: 
  * Inherits directly from the `Turtle` class.
  * Responsible for spawning food at random coordinates on the screen.
  * Uses the `refresh()` method to move to a new random location once eaten by the snake, taking care of hiding and showing itself for smooth animation.
* **`Score` (in `score_board.py`)**: 
  * Also inherits from the `Turtle` class.
  * Manages the current score and updates the UI text.
  * Persists the highest score to a file (`score.txt`), allowing the high score to be saved across different game sessions.
* **`main.py`**:
  * Acts as the game loop and orchestrates the components.
  * Initializes the screen and continuously listens for keyboard events.
  * Handles collision detection (with walls, the food, and the snake's own tail).

## How to Run
1. Make sure you have Python installed on your system.
2. Clone or download this repository.
3. Open a terminal or command prompt and navigate to the game's directory.
4. Execute the following command:
   ```bash
   python main.py
   ```
5. Use the **Up**, **Down**, **Left**, and **Right** arrow keys to control the snake.

Enjoy the game!
