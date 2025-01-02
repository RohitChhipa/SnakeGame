# Snake Game

This project is a classic Snake game implemented in Python using the Pygame library. The game is simple, engaging, and an excellent project for learning game development basics.

## Features

- **Classic Snake Gameplay**: The snake grows longer as it eats the food, and the game ends if it collides with the boundaries or itself.
- **Score Tracking**: Displays the current score dynamically on the screen.
- **Game Controls**:
  - Arrow keys to move the snake.
  - `C` to restart the game after losing.
  - `Q` to quit the game.

## Prerequisites

To run this game, ensure you have the following installed:

- Python 3.7 or higher
- Pygame library

Install Pygame using the command:
```bash
pip install pygame
```

## File Structure

```
SnakeGame/
├── main.py     # Main game logic
```

## Code Walkthrough

### Colors and Screen Setup

- Defined a palette of colors for the game elements (snake, food, background, etc.).
- Set the screen dimensions (600x400 pixels) and initialized the game window using Pygame.

### Game Mechanics

#### Snake Movement
- The snake is represented as a list of coordinates.
- Arrow keys control the direction of movement.

#### Food Generation
- The food appears randomly on the screen, and its position updates each time the snake eats it.

#### Collision Detection
- The game ends if:
  - The snake hits the boundaries of the screen.
  - The snake collides with itself.

### Functions

#### `display_score(score)`
- Displays the current score at the top-left corner of the screen.

#### `draw_snake(snake_block, snake_list)`
- Draws the snake on the screen using rectangles for each segment.

#### `message(msg, color)`
- Displays game-over or other informational messages at the center of the screen.

#### `game_loop()`
- The main game loop that handles:
  - Event handling (keyboard inputs).
  - Snake movement and growth.
  - Food consumption and regeneration.
  - Collision detection.
  - Updating the screen.

## Controls

- **Arrow Keys**: Move the snake up, down, left, or right.
- **C**: Restart the game after losing.
- **Q**: Quit the game.

## Running the Game

1. Clone or download the repository.
2. Navigate to the project directory.
3. Run the following command:
   ```bash
   python main.py
   ```
4. Enjoy the game!

## Example Output

- The snake moves in the direction of arrow keys.
- The score increases by 1 each time the snake eats the food.
- The game displays a "You Lost! Press C-Play Again or Q-Quit" message upon losing.

## Customization

- **Speed**: Adjust the `snake_speed` variable to increase or decrease the game's difficulty.
- **Snake Block Size**: Change the `snake_block` variable to modify the snake's size.
- **Screen Dimensions**: Update the `width` and `height` variables to resize the game window.

## License

This project is open-source and available under the MIT License.

---

Happy Coding! Enjoy playing and experimenting with this Snake Game!

