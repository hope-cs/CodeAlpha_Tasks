# 📧 Email Extractor
### CodeAlpha Python Programming Internship — Task 3 (Task Automation)

---

## 📖 Description

A Python automation script that scans any `.txt` file you provide, extracts all valid email addresses using **Regular Expressions (Regex)**, removes duplicates, and saves the results to a new output file. This is a real-world automation task that eliminates the need to manually search through large text files for email addresses.

This project demonstrates core Python automation concepts including file handling, regular expressions, functions, and set operations for duplicate removal.

---

## ✨ Features

- 🔍 **Regex Pattern Matching** — Uses a precise regular expression to detect all valid email formats
- 🚫 **Invalid Email Filtering** — Automatically ignores malformed entries like `@nouser`, `missingat.com`, `@@double.com`
- 🔄 **Duplicate Removal** — Uses Python `set()` to ensure each email appears only once
- 🔢 **Sorted Output** — Emails are sorted alphabetically for clean, readable results
- 💾 **Auto Save** — Saves all extracted emails to a `.txt` output file with a count summary
- 🖥️ **Console Display** — Shows numbered list of all found emails directly in the notebook
- ⚠️ **Error Handling** — Gracefully handles missing input file with a clear error message

---

## 🧠 Concepts Used

| Concept | Usage in This Project |
|---|---|
| `re` module | Built-in Python library for regular expressions |
| `re.findall()` | Finds all matches of the email pattern in the text |
| Regex pattern | Precisely matches valid email formats only |
| `set()` | Removes duplicate emails automatically |
| `sorted()` | Sorts emails alphabetically |
| `open()` / file handling | Reads input file and writes output file |
| `try/except` | Handles missing file error without crashing |
| `enumerate()` | Adds numbering to the displayed email list |
| Functions | Each task separated into its own reusable function |

---

## 🔍 Regex Pattern Explained

```
r'[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-]+'
```

| Part | What It Matches |
|---|---|
| `[a-zA-Z0-9_.+-]+` | Username — letters, numbers, dots, underscores, plus, hyphen |
| `@` | The required @ symbol |
| `[a-zA-Z0-9-]+` | Domain name — e.g. `gmail`, `yahoo`, `codealpha` |
| `\.` | The literal dot before the extension |
| `[a-zA-Z0-9-]+` | Extension — e.g. `com`, `org`, `tech`, `io` |

---

## 📁 Project Structure

```
CodeAlpha_EmailExtractor/
│
├── email_extractor.ipynb   # Main Jupyter Notebook — full automation script
├── emails_input.txt        # Your input file (place it in the same folder)
├── emails_output.txt       # Output file with extracted emails (auto-created)
├── README.md               # Project documentation (this file)
└── requirements.txt        # Python dependencies
```

---

## ⚙️ Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- No external libraries needed — uses built-in `re` and `os` modules only

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/YOUR_USERNAME/CodeAlpha_EmailExtractor.git
cd CodeAlpha_EmailExtractor
```

**2. Add your input file**
- Place your `.txt` file in the **same folder** as the notebook
- Rename it to `emails_input.txt` OR update this line in Cell 7:
```python
input_file = "your_file_name.txt"
```

**3. Launch Jupyter Notebook**
```bash
jupyter notebook email_extractor.ipynb
```

**4. Run the program**
- Open `email_extractor.ipynb` in Jupyter
- Run all cells from top to bottom (`Cell → Run All`)
- The last cell runs the full extraction automatically
- Results are saved to `emails_output.txt` in the same folder

---

## 🎮 How It Works — Step by Step

1. **Cell 1** imports the required built-in libraries `re` and `os`
2. **Cell 2** reads your input `.txt` file safely and returns its content
3. **Cell 3** scans the content using a regex pattern and extracts all valid emails
4. **Cell 4** saves the results neatly to `emails_output.txt`
5. **Cell 5** displays the numbered list of found emails in the console
6. **Cell 6** calls all functions in order and runs the full program

---

## 📸 Sample Output

```
🔍 Email Extractor Starting...

✅ File 'emails_input.txt' read successfully!

📧 Found 9 unique email(s):
========================================
  1. business.dev@company.org
  2. hr.department@careers.io
  3. hr2024@jobs.com
  4. jane_smith@yahoo.com
  5. john.doe123@gmail.com
  6. manager_2024@enterprise.org
  7. sales_team@corp.net
  8. support@codealpha.tech
  9. urgent@response.tech
========================================
✅ Emails saved to 'emails_output.txt'

✅ Done! Check 'emails_output.txt' for results.
```

---

## 🔧 Customization

You can easily extend this script by editing `email_extractor.ipynb`:

- **Use your own file** → Change `input_file = "emails_input.txt"` in Cell 6 to your own file name
- **Change output file name** → Modify `output_file = "emails_output.txt"` in Cell 6
- **Extract from multiple files** → Wrap `main()` in a loop over a list of file names

---

## 👨‍💻 Author

**Hamza Sajjad**
CodeAlpha Python Programming Intern
[GitHub Profile](https://github.com/hope-cs)

---

## 🏢 About CodeAlpha

CodeAlpha is a leading software development company providing internship programs focused on hands-on Python development experience.
[www.codealpha.tech](https://www.codealpha.tech)
