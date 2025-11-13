# Tic_Tac_Toe
Java console-based Tic-Tac-Toe game (CS3560 assignment)


# Tic Tac Toe (Java)

This is a simple console-based Tic Tac Toe game built in Java.

## Design Rationale
I separated the game into multiple classes so each part has one job:
- Board: stores the game state
- Game: controls the flow of the game
- Player: represents a person or AI
- ConsoleApp: runs the game

## How to Run
1. Open in IntelliJ
2. Run the `ConsoleApp` file
3. Play Tic Tac Toe in your console!

## Example Output
Welcome to Tic Tac Toe!
- - -
- - -
- - -
## Reflection

**Encapsulation:** Encapsulation prevented bugs by keeping the Board's grid private, ensuring that moves could only be applied through the place() method, which validates row, column, and cell occupancy.

**Inheritance:** Inheritance was used to create an abstract Player class and concrete HumanPlayer and RandomAIPlayer classes, allowing the Game to handle any type of player polymorphically without changing the game loop.

**Future Refactor:** If the rules changed to 4-in-a-row on a 5x5 board, I would refactor the Board class to allow a configurable size and winning condition, and update the winner() method to check for sequences of four instead of three.
