# Project Instructions: Snake Game (tkinter)

This project is a lightweight, dependency-free Snake game implemented in Python using the standard `tkinter` library.

## Project Overview
- **Purpose**: A simple, educational implementation of the classic Snake game.
- **Main Technologies**: 
  - **Language**: Python 3.x
  - **GUI Library**: `tkinter` (built-in)
- **Architecture**:
  - The game logic is contained within a single file (`snake.py`).
  - It uses a `Canvas` widget for drawing the snake and food.
  - The game loop is driven by the `window.after()` method to handle timing and movement.
  - Input is handled via keyboard event bindings for the arrow keys.

## Building and Running
### Run the Game
To start the game, execute the main script:
```powershell
python snake.py
```

### Testing
- **Automated Tests**: None currently implemented.
- **Manual Verification**: Launch the game and verify:
  - Arrow keys change direction correctly.
  - Snake grows when eating red circles (food).
  - Game ends when hitting walls or the snake's own body.
  - Score increments correctly.

## Development Conventions
### Code Style
- **Constants**: Defined at the top of `snake.py` in `UPPER_CASE`.
- **Naming**: Uses `snake_case` for functions and variables; `PascalCase` for classes (`Snake`, `Food`).
- **Structure**:
  - Constants define game parameters (speed, dimensions, colors).
  - Classes manage object state and initial rendering.
  - Global functions handle game loop logic and collision detection.

### Guidelines for Changes
- **Configuration**: Always check constants like `SPEED` or `SPACE_SIZE` before modifying game behavior.
- **Rendering**: Updates to the snake's visual state should be handled within `next_turn` by creating and deleting canvas objects.
- **Dependencies**: Maintain the "no-external-dependency" requirement by only using Python standard library modules.
