#Intro to Java Programming Project - Tic Tac Toe!


##Summary

In this project, you are required to complete the code for a Tic-Tac-Toe game, the source code of the game GUI and computer logic can be downloaded [here](https://github.com/udacity/ud282) and you can start compiling and playing straight away, however, you will notice the code is not complete because the game never detects the winner!


##Rules of the Game

Tic-Tac_Toe is a 2 player board game, one plays as X and the other plays as O, the board is a 3x3 grid where each cell can either be marked X or O, starting with an empty grid, each player takes turns to mark a blank cell with either X or O depending on which player they are, the goal for the X player is to get 3 X’s in one line either vertically, horizontally or diagonally, same goes for the O player.

Once a line is formed the game ends and the player who formed that line wins! However more than likely, especially if both players are good, all cells could end up marked with X’s and O’s with no lines, hence no winner, this game ends as a tie.


##Code design

The [source code](https://github.com/udacity/ud282/tree/master/Project%201%20-%20TicTacToe) includes 2 main Java files in `src/main/java/com/udacity`, `Game.java` and `GameUI.java`.  `Game.java` is where all the game logic code exists, while `GameUI.java` is where all the user interface code exists.  You can take a look at GameUI.java if you like, but it is not necessary to change any code there to complete the project.  Your job is to implement the `checkGameWinner()` function in `Game.java` file.

The function `public String checkGameWinner(char [][] grid)` has a 2D char array as an input representing the game grid (see below for details) and it returns a String message indicating which player has won (X wins , O wins, Tie, or None if the game hasn't ended yet).  The contents of the `grid` array correspond to the boxes in the Tic-Tac-Toe grid like this:

               |            |
    grid[0][0] | grid[1][0] | grid[2][0]
               |            |
    ------------------------------------
               |            |
    grid[0][1] | grid[1][1] | grid[2][1]
               |            |
    ------------------------------------
               |            |
    grid[0][2] | grid[1][2] | grid[2][2]
               |            |


`doChecks()` is another function that is responsible for calling `checkGameWinner()` every time a player takes a turn, so you should not worry about fitting this function into the rest of the program.  This is already taken care of.

The Grid is represented as a 2D array of characters, indexed as follows:


##Requirements

In `checkGameWinner()` you should access those cells in the 2D array to find out if either X or O or neither has won the game by checking if there’s 3 of the same kind in a row either horizontally, vertically or diagonally!

- If you detect a winner, set the variable result to either `"X wins"` or `"O wins"` depending on the player who won.
- If the game ends as a tie, set result to `"Tie"`.
- If the game has not ended yet set result to `"None"`.

Then make sure the function would return that variable result at the end (you can also return the String literal directly as you detect a winner or tie).

You are allowed to create and use extra functions if you want you, but you do not need to do so.

Make sure you test the code by playing the game many times with all the different possible scenarios of winning. If you find a bug, remember that you can use the debugging feature in IntelliJ that would help trace and follow your code and point you to the right direction.

Once you’re happy with your code, you should submit the entire project directory as a .zip folder.