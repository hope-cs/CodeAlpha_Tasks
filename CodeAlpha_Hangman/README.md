# 🎮 Hangman Game
### CodeAlpha Python Programming Internship — Task 1

---

## 📖 Description

A classic text-based **Hangman Game** built entirely in Python and designed to run inside a **Jupyter Notebook**. The player tries to guess a hidden word one letter at a time. With every wrong guess, a new body part is drawn on the hangman gallows. The game ends when the player either guesses the full word correctly or exhausts all 6 attempts.

This project demonstrates core Python fundamentals including randomization, loops, sets, input validation, and clean terminal UI using `clear_output` for a smooth, non-scrolling game experience.

---

## ✨ Features

- 🎲 **Random Word Selection** — Picks a different word every game from a predefined list
- 🖼️ **Live Hangman Drawing** — ASCII art gallows builds step by step with each wrong guess (7 stages total)
- 🔡 **Word Progress Display** — Correctly guessed letters are revealed; unguessed letters shown as `_`
- 📋 **Guess Tracker** — Displays all guessed letters so far, sorted alphabetically
- ✅ **Input Validation** — Rejects numbers, symbols, multiple characters, and duplicate guesses
- 🔄 **Clean Screen Refresh** — Uses `clear_output(wait=True)` so each round replaces the previous output instead of stacking
- 💬 **Live Feedback Messages** — Shows result of each guess on the same refreshed screen
- 🏆 **Win / Loss Detection** — Automatically detects when the player wins or runs out of guesses

---

## 🧠 Concepts Used

| Concept | Usage in This Project |
|---|---|
| `random.choice()` | Randomly selects a word from the list each game |
| `set` | Stores guessed letters — prevents duplicates, fast lookup |
| `while loop` | Keeps the game running until win or loss condition |
| `if-elif-else` | Handles all game conditions (correct, wrong, duplicate, invalid) |
| `all()` | Checks if every letter in the word has been guessed (win check) |
| String methods | `.lower()`, `.strip()`, `.isalpha()` for clean input handling |
| `clear_output()` | IPython function to refresh Jupyter cell output each round |
| f-strings | Clean, readable dynamic output formatting |
| Functions | `display_word()` separates display logic from game logic |

---

## 📁 Project Structure

```
CodeAlpha_HangmanGame/
│
├── hangman.ipynb       # Main Jupyter Notebook — full game code
├── README.md           # Project documentation (this file)
├── requirements.txt    # Python dependencies
└── .gitignore          # Files ignored by Git
```

---

## ⚙️ Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- IPython (comes pre-installed with Jupyter)

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/hope-cs/CodeAlpha_Hangman.git
cd CodeAlpha_Hangman
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Launch Jupyter Notebook**
```bash
jupyter notebook hangman.ipynb
```

**4. Run the game**
- Open `hangman.ipynb` in Jupyter
- Run all cells from top to bottom (`Cell → Run All`)
- The last cell starts the game — type your letter guesses in the input box

---

## 🎮 How to Play

1. The game picks a **random hidden word** and shows blanks (`_`) for each letter
2. Type **one letter** at a time and press Enter
3. ✅ **Correct guess** → the letter is revealed in the word
4. ❌ **Wrong guess** → a body part is added to the hangman drawing
5. You get a maximum of **6 wrong guesses**
6. **Win** by guessing all letters before the hangman is complete
7. **Lose** if the hangman is fully drawn before you guess the word

---

## 📸 Sample Output

```
========================================
       🎮 Hangman Game
========================================

       -----
       |   |
       O   |
      /|\  |
           |
           |
    =========

Word:  p _ _ _ _ _
Wrong guesses left: 3
Letters guessed: a, e, o, p, z

✅ Nice! 'p' is in the word!

Guess a letter: _
```

---

## 🔧 Customization

You can easily extend this game by editing `hangman.ipynb`:

- **Add more words** → Edit the `WORDS` list
- **Change difficulty** → Modify `max_wrong` (lower = harder)
- **Add categories** → Create multiple word lists (animals, countries, tech terms etc.)

---

## 👨‍💻 Author

**Ali**
CodeAlpha Python Programming Intern
[GitHub Profile](https://github.com/hope-cs)

---

## 🏢 About CodeAlpha

CodeAlpha is a leading software development company providing internship programs focused on hands-on Python development experience.
[www.codealpha.tech](https://www.codealpha.tech)
