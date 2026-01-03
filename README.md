# Tic-Tac-Toe Game

## Overview

This is a simple console-based Tic-Tac-Toe game implemented in C++. The game allows a human player to compete against a computer opponent. The player uses 'X' and the computer uses 'O'. The game features a basic AI that makes random moves, checks for wins, losses, and ties, and provides a visual representation of the game board in the terminal.

## Features

- **Player vs Computer**: Play against a computer opponent that makes random moves.
- **Visual Board**: The game board is displayed in the console with a simple ASCII art representation.
- **Win/Loss Detection**: Automatically detects and announces wins, losses, and ties.
- **Input Validation**: Ensures valid moves and handles invalid inputs gracefully.
- **Turn-Based Gameplay**: Alternates between player and computer turns.

## Game Rules

- The game is played on a 3x3 grid.
- The player (X) goes first, followed by the computer (O).
- Players take turns placing their mark on an empty space.
- The first to get three of their marks in a row (horizontally, vertically, or diagonally) wins.
- If all spaces are filled without a winner, it's a tie.

## How to Play

1. The game starts with an empty board.
2. You will be prompted to enter a number from 1 to 9 corresponding to the board positions:
   ```
       |       |
    1  |  2    |  3
   ____|_______|____
       |       |
    4  |  5    |  6
   ____|_______|____
       |       |
    7  |  8    |  9
       |       |
   ```
3. Enter your move by typing the number and pressing Enter.
4. The computer will make its move automatically.
5. The game continues until there's a winner or a tie.

## Installation and Compilation

### Prerequisites

- A C++ compiler (e.g., g++ for Windows, which can be installed via MinGW or MSYS2).
- On Windows, you can install MinGW from [mingw-w64.org](https://mingw-w64.org/) or use Visual Studio with C++ support.

### Compilation Steps

1. Ensure you have a C++ compiler installed and accessible from the command line.
2. Navigate to the `src` directory of the project:
   ```
   cd Tic-Tac-Toe/src
   ```
3. Compile the source code using g++:
   ```
   g++ TicTacToe.cpp -o TicTacToe.exe
   ```
   This will generate an executable file named `TicTacToe.exe`.

### Running the Game

After compilation, run the executable:
```
TicTacToe.exe
```

## Code Structure

- `TicTacToe.cpp`: The main source file containing all game logic.
  - `drawBoard()`: Displays the current state of the game board.
  - `playerMove()`: Handles player input and updates the board.
  - `computerMove()`: Generates a random move for the computer.
  - `checkWinner()`: Checks for winning conditions and announces the result.
  - `checkTie()`: Checks if the game is a tie.
  - `main()`: The entry point that runs the game loop.

## Example Gameplay

```
      |       |
   1  |  2    |  3
_____|_______|_____
      |       |
   4  |  5    |  6
_____|_______|_____
      |       |
   7  |  8    |  9
      |       |

 Input any number ranging from 1 to 9 : 5

      |       |
   1  |  2    |  3
_____|_______|_____
      |       |
   4  |  X    |  6
_____|_______|_____
      |       |
   7  |  8    |  9
      |       |

[Computer makes a move...]

      |       |
   1  |  2    |  O
_____|_______|_____
      |       |
   4  |  X    |  6
_____|_______|_____
      |       |
   7  |  8    |  9
      |       |

[Game continues...]
```

## Contributing

Feel free to fork this repository and submit pull requests for improvements, bug fixes, or new features. Suggestions for enhancing the AI (e.g., implementing minimax algorithm) are welcome.

## License

This project is open-source and available under the MIT License. See the LICENSE file for more details (if applicable).

## Author

Developed by [Your Name or Anonymous]. For questions or feedback, please open an issue in the repository.
