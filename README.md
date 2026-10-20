# Number Guessing Games

Two small Python scripts for number guessing games, played in the terminal. No dependencies beyond the standard library (Python 3.6+).

## Scripts

| File | What it does |
|------|--------------|
| `guess_the_number(computer).py` | Contains two games: `guess(x)` (you guess the computer's number) and `computer_guess(x)` (the computer guesses yours). Runs `computer_guess(50)` by default. |
| `guess_the_number(user).py` | A simpler version: you guess a random number between 1 and 10. |

## Usage

```bash
guess_the_number(user).py
guess_the_number(computer).py
```

### You guess the number (`guess_the_number(user).py`)

The computer picks a random number from 1 to 10. Keep guessing; it tells you if you're too low or too high until you get it.

```
Guess a number between 1 and 10: 5
Sorry, guess again. Too low.
```

### The computer guesses your number (`guess_the_number(computer).py`)

Think of a number between 1 and 50. The computer guesses, and you reply:

- `H` if the guess is too high
- `L` if the guess is too low
- `C` if it's correct

```
Is 23 too high (H), too low (L), or correct (C)? h
```

## Customizing

- Change the range by editing the argument in the last line of each script, e.g. `guess(100)` or `computer_guess(200)`.
- To play "you guess" in `guess_the_number(user).py`, replace the last line with `guess(10)`.

## Notes

- Enter whole numbers only when guessing; anything else raises a `ValueError`.
- In `guess_the_number(computer).py`, answer honestly. If your replies contradict each other, the computer can run out of valid numbers and crash.

## Author

Eve Mertic
