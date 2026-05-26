# 📈 Stock Portfolio Tracker
### CodeAlpha Python Programming Internship — Task 2

---

## 📖 Description

A simple yet functional **Stock Portfolio Tracker** built in Python and designed to run inside a **Jupyter Notebook**. The user inputs stock symbols and quantities, and the program automatically calculates the total investment value based on hardcoded stock prices. Results can optionally be saved to a `.csv` or `.txt` file for future reference.

This project demonstrates core Python fundamentals including dictionaries, functions, loops, input validation, file handling, and clean terminal UI using `clear_output` for a smooth experience.

---

## ✨ Features

- 📋 **Available Stocks Display** — Shows all supported stock symbols and their prices in a neat table before input
- ✅ **Real-time Entry Confirmation** — After each stock entry, instantly shows symbol, quantity, price per share and total value
- 🔍 **Input Validation** — Rejects invalid stock symbols, negative quantities, and non-numeric input without crashing
- 📊 **Portfolio Summary Table** — Displays a clean breakdown of all entered stocks with individual and total investment values
- 💾 **File Saving** — Optionally saves the portfolio report to a `.csv` or `.txt` file
- 🔄 **Multiple Portfolios** — Option to track another portfolio without restarting the program
- 🖥️ **Clean Screen Refresh** — Uses `clear_output(wait=True)` to keep the display clean and non-scrolling

---

## 🧠 Concepts Used

| Concept | Usage in This Project |
|---|---|
| `dictionary` | Stores hardcoded stock prices for fast lookup |
| `functions` | Each task separated into its own reusable function |
| `while loop` | Keeps accepting stock entries until user types `done` |
| `try/except` | Handles invalid quantity input without crashing |
| `f-strings` | Clean, readable dynamic output formatting |
| `string alignment` | `:<10` and `:>12` for neat table formatting |
| `csv module` | Saves portfolio data to a `.csv` file |
| `file handling` | Writes portfolio report to a `.txt` file |
| `clear_output()` | IPython function to refresh Jupyter cell output |

---

## 📁 Project Structure

```
CodeAlpha_StockPortfolioTracker/
│
├── stock_tracker.ipynb     # Main Jupyter Notebook — full program code
├── README.md               # Project documentation (this file)
└── requirements.txt        # Python dependencies
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
git clone https://github.com/hope-cs/CodeAlpha_Tasks.git
cd CodeAlpha_Tasks/CodeAlpha_StockPortfolioTracker
```

**2. Install dependencies**
```bash
pip install -r requirements.txt
```

**3. Launch Jupyter Notebook**
```bash
jupyter notebook stock_tracker.ipynb
```

**4. Run the program**
- Open `stock_tracker.ipynb` in Jupyter
- Run all cells from top to bottom (`Cell → Run All`)
- The last cell starts the program

---

## 🎮 How to Use

1. The program displays all **available stock symbols** and their prices
2. Enter a **stock symbol** (e.g. `AAPL`) and press Enter
3. Enter the **quantity** of shares you own and press Enter
4. Instantly see a confirmation of your entry with its value
5. Repeat for more stocks
6. Type `done` when finished
7. View your complete **portfolio summary** with total investment
8. Choose to save as **CSV**, **TXT**, or skip saving

---

## 📈 Supported Stocks

| Symbol | Company | Price (USD) |
|---|---|---|
| AAPL | Apple Inc. | $180 |
| TSLA | Tesla Inc. | $250 |
| GOOGL | Alphabet Inc. | $140 |
| AMZN | Amazon.com Inc. | $185 |
| MSFT | Microsoft Corp. | $420 |

---

## 📸 Sample Output

```
📈 Available Stocks:
Symbol        Price (USD)
------------------------
AAPL                $180
TSLA                $250
GOOGL               $140
AMZN                $185
MSFT                $420

💼 Enter your stock holdings (type 'done' to finish):
Stock symbol: AAPL
Quantity of AAPL: 10
✅ Added 10 shares of AAPL @ $180 = $1,800
----------------------------------------
Stock symbol: TSLA
Quantity of TSLA: 5
✅ Added 5 shares of TSLA @ $250 = $1,250
----------------------------------------
Stock symbol: done

📊 Portfolio Summary:
Symbol          Qty      Price        Value
------------------------------------------
AAPL             10       $180       $1,800
TSLA              5       $250       $1,250
------------------------------------------
            TOTAL INVESTMENT       $3,050
```

---

## 🔧 Customization

You can easily extend this program by editing `stock_tracker.ipynb`:

- **Add more stocks** → Edit the `STOCK_PRICES` dictionary in Cell 2
- **Update prices** → Change the values in `STOCK_PRICES`
- **Add more file formats** → Extend the `save_to_file()` function

---

## 👨‍💻 Author

**Hamza Sajjad**
CodeAlpha Python Programming Intern
[GitHub Profile](https://github.com/hope-cs)

---

## 🏢 About CodeAlpha

CodeAlpha is a leading software development company providing internship programs focused on hands-on Python development experience.
[www.codealpha.tech](https://www.codealpha.tech)
