# Tic Tac Tow with AI

This is a python implementation of the paper-and-pencil game from childhood: Tic-Tac-Toe, also known as Noughts and crosses or 
Xs and Os.

This project is from the **Jetbrain Academy** (https://www.jetbrains.com/academy/).
 
## Features

It is possible to play the game with the AI, with three levels.

The "**easy**" level will make random moves.

The "**medium**" level difficulty makes a move using the following process:

    1. If it can win in one move (if it has two in a row), it places a third to get three in a row and win.
    2. If the opponent can win in one move, it plays the third itself to block the opponent to win.
    3. Otherwise, it makes a random move. 

The "**hard**" level difficulty implements the **minimax** algorithm, which is the brute force algorithm that maximizes the 
value of the own position and minimizes the value of the opponent's position. Basically, it can see all possible 
outcomes till the end of the game and choose the best of them considering his opponent also would play perfectly. So, it 
does not rely on the blunders of the opponent, it plays perfectly regardless of the opponent's skill.

 
## Usage

Download the repository and run tic-tac-tow.py.

The main menu accepts two commands: "**start**" and "**exit**". The "start" command takes two parameters: four parameters are 
possible: "**user**" to play as a human, and "**easy**", "**medium**" and "**hard**" to play as an easy level AI.
The command "exit" should simply terminate the program.

The first player uses the "X" symbol, the second "O".

If any of the player is human, the user should input 2 numbers that represent the cell on which user wants to make his 
"X" or "O".

```
Input command: > start user hard
---------
|       |
|       |
|       |
---------
Enter the coordinates: (x y) > 2 2
---------
|       |
|   X   |
|       |
---------
Making move level "hard"
---------
|     O |
|   X   |
|       |
---------
Enter the coordinates: (x y) > 
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.
