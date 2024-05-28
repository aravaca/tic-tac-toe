# About Tic-tac-toe

This project includes a classic 3x3 tic-tac-toe game where you play against an invincible AI computer. The AI uses the minimax algorithm and computes heuristic values (in other words, it looks ahead moves) to make the optimal choice.

## Description

To play the game on Windows, simply download the tic-tac-toe AI.exe file in the dist folder and run it. Otherwise, assuming that you have Python installed, copy the source code (or clone the repository) and run the game using the following command:
```bash
python game.py
```
Then, follow the instructions as you play.

NOTE:
The grid uses 1-9 indexing from left to right in the following form:<br/>
1 | 2 | 3<br/>
4 | 5 | 6<br/>
7 | 8 | 9<br/>

## Acknowledgement
The source code for the basic version of the game is from Kylie Ying's GitHub (https://github.com/kying18). I want to give a special thanks to her wonderful YouTube tutorial. However, the class AI_Player in player.py, method get_owl in game.py, and the main method, which contains all necessary logic and procedures for the AI and its algorithm, are solely written on my own. I have also added features such as a scoreboard, choosing the order in which player goes first, and playing again. For the minimax algorithm and heuristic function, I referred to notes from Justin Wyss-Gallifent (https://math.umd.edu/~immortal/). I want to give a special thanks to his wonderful detailed notes.


