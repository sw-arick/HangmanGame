# Hangman Game

A command-line Hangman game written in Python. The computer picks a random fruit, and you guess it one letter at a time. Every wrong guess adds a piece to the ASCII hangman, and you lose when the drawing is complete.

## Features

- Random fruit picked from a built-in word list on every run
- Hint at the start telling you the word is a fruit
- ASCII hangman art that updates with each wrong guess
- 6 wrong guesses allowed
- Input validation: non-letters, multiple characters, and repeated guesses don't cost an attempt
- Win and game over messages that reveal the word

## How to play

1. Run the program.
2. Guess one letter at a time.
3. Correct letters fill in the blanks; wrong letters add to the hangman.
4. Reveal the whole word before the drawing is finished.

## Example

```
Welcome to Hangman!
Hint: The word is a fruit.

     -----
     |   |
         |
         |
         |
    =========

Word: _ _ _ _ _
Guess a letter: a
Correct guess!
```

## Run it locally

```bash
git clone https://github.com/sw-arick/hangman-game.git
cd hangman-game
python hangman.py
```

Requires Python 3. No external libraries needed.

## Concepts used

- `random.choice()` for picking a word
- Lists for storing the ASCII art stages and guessed letters
- `while` loop with an `else` clause for the lose condition
- String building to display the partially guessed word
- Input validation with `isalpha()` and `len()`

## Ideas for improvement

- Add a "play again" option
- Add word categories (animals, countries, tech) with matching hints
- Load words from a text file
- Add difficulty levels with different word lengths
- Keep a score across rounds

## Author

[sw-arick](https://github.com/sw-arick)
