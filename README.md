# Higher Luck – Project 1

OOP course project, Fall 2026 (Vistula University)
Team: **[Your Group Name]**
Members: [Name Surname], [Name Surname], [Name Surname]

## What is it?

A simple two-player dice game made in C# with Windows Forms. Each round both
players roll a die and whoever gets the higher number gets a point. If both roll
the same number, they both get a point. After the last round the winner is shown
and the result is saved to a txt file.

## How to play

1. Pick the number of rounds (5 to 30).
2. Type in both player names. The setup buttons unlock once the names are filled in.
3. Choose an avatar and click **Set Up First Player**, then pick a different avatar
   and click **Set Up Second Player**. You can't pick the same avatar twice.
4. Click **START**.
5. Players take turns clicking **ROLL**. The black label shows whose turn it is.
6. When all rounds are done, a message box shows the winner and the game resets.

Other buttons:
- **SHOW RESULT** loads all past games from the txt file into the Report list.
- **RESET ALL** clears everything and starts over, at any time.

## How it works (short version)

- `Player` class keeps each player's name, avatar and points.
- Results are saved to `results.txt` (no database, just file operations).
  Each line looks like: `NAME1;points;NAME2;points;The winner is NAME`
- Avatar and dice images are stored in the project's Resources, so they work on
  any computer without changing file paths.
- File reading/writing is wrapped in try-catch so the app doesn't crash if
  something goes wrong with the file.

## How to run

1. Open the `.sln` file in Visual Studio.
2. Build and run (F5).
3. That's it. `results.txt` is created automatically after the first game.
