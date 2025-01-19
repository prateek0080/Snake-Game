# Snake Game

A classic Snake Game implementation in Java using Swing graphics. The player controls a snake that grows longer as it eats apples while avoiding collisions with walls and itself.

## Features

- Smooth snake movement with arrow key controls
- Random apple generation
- Score tracking through snake length
- Game over detection for wall and self-collision
- Clean and responsive UI
- Custom graphics for snake head, body, and apple

## Requirements

- Java Development Kit (JDK) 8 or higher
- Java Runtime Environment (JRE)

## Project Structure

```
snakegame/
│
├── SnakeGame.java    # Main game class with JFrame setup
├── Board.java        # Game logic and rendering
│
└── icons/
    ├── apple.png     # Apple sprite
    ├── dot.png       # Snake body sprite
    └── head.png      # Snake head sprite
```

## How to Play

1. Run the game using `java snakegame.SnakeGame`
2. Use arrow keys to control the snake's direction:
   - ↑ (Up Arrow): Move up
   - ↓ (Down Arrow): Move down
   - ← (Left Arrow): Move left
   - → (Right Arrow): Move right
3. Eat apples to grow longer
4. Avoid hitting the walls or the snake's own body
5. Try to achieve the highest possible score!

## Game Rules

- The snake starts with a length of 3 segments
- Each apple eaten increases the snake's length by one segment
- The game ends if the snake:
  - Hits the wall boundaries
  - Collides with its own body
  - The game speed remains constant throughout gameplay

## Controls

| Key           | Action        |
|---------------|---------------|
| ← Left Arrow  | Move left     |
| → Right Arrow | Move right    |
| ↑ Up Arrow    | Move up       |
| ↓ Down Arrow  | Move down     |

## Technical Details

- Window Size: 300x300 pixels
- Grid Size: 10x10 pixels per cell
- Game Timer: 140ms refresh rate
- Written in Java using Swing framework
- Implements `ActionListener` for game loop
- Uses `KeyAdapter` for input handling

