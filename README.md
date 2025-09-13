# Tic-Tac-Toe AI Game 🎮

A Python-based Tic-Tac-Toe game featuring an intelligent AI opponent powered by the minimax algorithm. This interactive game offers multiple gameplay modes and a clean, modern graphical interface.

![Game Screenshot](tic-tac-toe-ai.png)

## 🌟 Features

- **Smart AI Opponent**: Implements the minimax algorithm for optimal gameplay
- **Multiple Game Modes**:
  - Player vs. Smart AI (minimax algorithm)
  - Player vs. Random AI
  - Player vs. Player (local multiplayer)
- **Clean GUI**: Modern interface built with Pygame
- **Real-time Gameplay**: Smooth animations and responsive controls
- **Game State Management**: Win detection with visual indicators
- **Easy Mode Switching**: Switch between different AI difficulty levels during gameplay

## 🎯 Game Modes

### 1. Smart AI Mode (Default)

The AI uses the minimax algorithm to make optimal moves, providing a challenging experience for players of all skill levels.

### 2. Random AI Mode

The AI makes random moves, perfect for casual gameplay or beginners.

### 3. Player vs Player Mode

Two human players can play against each other on the same device.

## 🎮 Controls

| Key           | Action                                           |
| ------------- | ------------------------------------------------ |
| `Mouse Click` | Place your mark (X or O) on the grid             |
| `G`           | Toggle between AI mode and Player vs Player mode |
| `R`           | Restart the game                                 |
| `0`           | Set AI to random mode                            |
| `1`           | Set AI to smart mode (minimax)                   |

## 📋 Requirements

- Python 3.6+
- pygame
- numpy

## 🚀 Installation & Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Cydonia01/Tic-Tac-Toe-AI.git
   cd Tic-Tac-Toe-AI
   ```

2. **Install required dependencies:**

   ```bash
   pip install pygame numpy
   ```

3. **Run the game:**
   ```bash
   python main.py
   ```

## 🎲 How to Play

1. **Starting the Game**: Run `main.py` to start the game
2. **Making Moves**: Click on any empty square to place your mark
3. **Player Symbols**:
   - Player 1: X (Cross) - Dark gray color
   - Player 2/AI: O (Circle) - Light cream color
4. **Winning**: Get three of your symbols in a row (horizontally, vertically, or diagonally)
5. **Game Over**: The game ends when someone wins or the board is full (draw)

## 🏗️ Project Structure

```
Tic-Tac-Toe-AI/
│
├── main.py           # Main game logic and execution
├── constants.py      # Game constants (colors, dimensions, etc.)
├── README.md         # Project documentation
└── tic-tac-toe-ai.png # Game screenshot
```

## 🧠 AI Algorithm

The smart AI uses the **minimax algorithm** with the following approach:

- **Evaluation Function**:
  - +1 for AI win
  - -1 for player win
  - 0 for draw
- **Decision Making**: The AI explores all possible future game states to choose the optimal move
- **Optimization**: Uses recursive tree traversal to evaluate the best possible outcome

## 🎨 Customization

You can easily customize the game by modifying `constants.py`:

- **Window Size**: Adjust `WIDTH` and `HEIGHT`
- **Grid Size**: Modify `ROWS` and `COLS` for different grid sizes
- **Colors**: Change `BG_COLOR`, `LINE_COLOR`, `CIRC_COLOR`, `CROSS_COLOR`
- **Dimensions**: Adjust line widths, circle radius, and offsets

## 🔧 Technical Details

### Classes:

- **Board**: Manages the game board state, win detection, and move validation
- **AI**: Implements both random and minimax AI strategies
- **Game**: Handles game flow, player turns, and rendering

### Key Features:

- **Win Detection**: Checks for horizontal, vertical, and diagonal wins
- **State Management**: Tracks empty squares and game completion
- **Visual Feedback**: Highlights winning combinations
- **Responsive Design**: Adapts to different screen sizes
