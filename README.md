# Higher Luck - Project 1

OOP course, Vistula University, 2026

Members:
- Lazizbek Sultonov (79244)
- Oualid Kesraoui (78482)
- Damian Barczewski (78985)

## About the game

This is a dice game for 2 players written in C# (Windows Forms). Every round
each player rolls the dice. The player with the bigger number gets 1 point.
If the numbers are the same both players get 1 point. When all rounds are
finished the program shows who won and saves the result into a txt file.

## How to play

1. Choose how many rounds you want (from 5 to 30).
2. Write the names of player 1 and player 2. Buttons for setup are disabled
   until both names are written.
3. Select an avatar and press "Set Up First Player". Then select another avatar
   and press "Set Up Second Player". Two players cannot have the same avatar.
4. Press "START".
5. Press "ROLL" one by one. The black label says which player should roll now.
6. After the last round a message box shows the winner and the game goes back
   to the start.

There are also 2 more buttons:
- "SHOW RESULT" - reads the txt file and shows all old games in the Report list.
- "RESET ALL" - clears everything, you can press it any time.

## How it is made

- There is a Player class which stores name, avatar and points of a player.
- Results are saved in results.txt. We don't use a database, only file
  read/write. One line in the file looks like this:
  NAME1;points;NAME2;points;The winner is NAME
- Pictures of avatars and dice are in the Resources of the project, so we
  don't need to change paths on another computer.
- Reading and writing the file is inside try-catch, so if there is some
  problem with the file the program will not crash.

## How to run

Open the .sln file in Visual Studio and press F5. The file results.txt will be
created by itself after the first game.
