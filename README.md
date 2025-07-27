# Tic-Tac-Toe Game

This project implements a simple Tic-Tac-Toe game where the player competes against the computer. The computer uses the **Minimax algorithm** to decide its moves, ensuring optimal gameplay. The game is played on a 3x3 grid, and the first player to align three of their symbols (horizontally, vertically, or diagonally) wins the game.

---

## Features

1. **Player vs Computer**:
   - The player uses 'X'.
   - The computer uses 'O'.
2. **Minimax Algorithm**:
   - The computer evaluates all possible moves to make the best decision.
3. **Interactive Gameplay**:
   - Players choose their moves by entering numbers corresponding to grid cells.
   - The game updates the board and provides feedback for invalid moves.
4. **Game End Conditions**:
   - The game declares a winner when three symbols align.
   - The game ends in a draw if the board is full without a winner.
5. **Randomized Moves for Fairness**:
   - Move order is randomized during initialization to provide variety.

---

## How to Play

1. **Board Setup**:
   - The game board is displayed as a 3x3 grid.
   - Each cell is numbered as follows:
     ```
      1 | 2 | 3
     -----------
      4 | 5 | 6
     -----------
      7 | 8 | 9
     ```

2. **Player Turn**:
   - Enter the number corresponding to the cell where you want to place your move ('X').
   - If the chosen cell is already occupied or invalid, you'll be prompted to try again.

3. **Computer Turn**:
   - The computer analyzes the board and places 'O' in the optimal cell.

4. **Winning and Draws**:
   - The game announces the winner when a row, column, or diagonal is filled with the same symbol.
   - If all cells are filled without a winner, the game ends in a draw.

---

## Code Structure

### Key Components

1. **Minimax Algorithm**:
   - `evaluate()`: Evaluates the board and assigns a score (+10 for player win, -10 for computer win, 0 otherwise).
   - `minimax()`: Recursively evaluates possible moves to find the optimal outcome.
   - `findBestMove()`: Identifies the best move for the computer.

2. **Game Functions**:
   - `initialise()`: Sets up the board and randomizes move order.
   - `showBoard()`: Displays the current state of the board.
   - `gameOver()`: Checks if the game has ended due to a win or draw.
   - `declareWinner()`: Announces the winner.

3. **Main Functionality**:
   - `playTicTacToe()`: Handles the game loop, alternating turns between the player and computer until the game ends.

---

## How to Run the Program

1. **Compile the Code**:
   Use any C compiler to compile the program. For example:
   ```bash
   gcc tic_tac_toe.c -o tic_tac_toe
   ```

2. **Run the Game**:
   Execute the compiled program:
   ```bash
   ./tic_tac_toe
  

3. **Follow Instructions**:
   The program will guide you to make your moves and display the game board after every turn.

---

## Improvements and Extensions

- Add a user-friendly graphical interface.
- Allow the player to choose their symbol ('X' or 'O').
- Enable two-player mode for playing against another human.
- Implement difficulty levels for the computer.
- Expand the grid size (e.g., 4x4 or 5x5) to increase complexity.

---

## Acknowledgments

The game leverages the Minimax algorithm to ensure competitive gameplay, making it an excellent example of AI in action.

---

Enjoy playing Tic-Tac-Toe against an intelligent opponent!


