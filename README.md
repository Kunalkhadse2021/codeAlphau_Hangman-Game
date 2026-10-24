# Hangman Game

A simple command-line Hangman game written in Python.

## Overview

This project lets players guess a hidden word letter by letter. Each incorrect guess increases the number of wrong attempts, and the game ends when the player either guesses the word correctly or runs out of chances.

## Features

- Random word selection from a built-in list
- Letter-by-letter guessing
- Wrong-attempt tracking
- Win/lose messages
- Option to play again after each round

## How to Run

1. Make sure Python 3 is installed on your system.
2. Save the game script as `hangman.py`.
3. Run:

```bash
python hangman.py
```

## Gameplay

- The game displays the word with underscores for hidden letters.
- Enter one letter at a time.
- If the letter is in the word, it is revealed.
- If not, the number of wrong guesses increases.
- You win by guessing all letters before the allowed attempts are exhausted.

## Example

```text
Welcome to Hangman!
Guess the hidden word one letter at a time.

Word: _ _ _ _ _
Wrong guesses left: 6
Enter a letter: a
Correct!
```

## Project Structure

- `hangman.py` — main game logic

## License

This project is provided for educational purposes.
