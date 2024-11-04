# 💻Project: Number Guessing Game

## Project Goal
Use Bash scripting, PostgreSQL, and Git to create a number guessing game that runs in the terminal and saves user information.

Project made as part of the FreeCodeCamp Relational Databases Certificate course

# Process
Database was created in PostgreSQL to insert and store user information and game history.

Tables:
<ul>
  <li>'games' - stores game history, including the user_id, the number of guesses inputed before finishing game and the 'secret number'.</li>
  <li>'users' - stores usernames (and corresponding user_id) so bash script will recognised new and returning users.</li>
</ul>

The Bash script runs the game until the 'secret number' is correctly guessed.

Based on the user input, it will hint whether the guess made is lower or higher than the 'secret number'.

The script recognised if the users are new or returning players based on their username and updates the database anytime a new user is detected.

It also updates and stores the game history for both new and returning players, including total number of games played and the best record for fewest number of guesses it took for user to win the game.
