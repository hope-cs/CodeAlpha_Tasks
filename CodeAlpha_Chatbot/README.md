# 🤖 PyBot — Rule-Based Chatbot
### CodeAlpha Python Programming Internship — Task 4

---

## 📖 Description

A simple yet interactive **Rule-Based Chatbot** built entirely in Python and designed to run inside a **Jupyter Notebook**. PyBot responds to user messages using predefined keyword matching rules — no AI or machine learning involved. The chatbot maintains a full chat history that is displayed and refreshed after every message, giving it a clean messenger-like feel.

This project demonstrates core Python fundamentals including dictionaries, functions, loops, string matching, and dynamic responses.

---

## ✨ Features

- 💬 **Keyword-Based Responses** — Matches user input against grouped keywords to find the best response
- 🕐 **Dynamic Time Response** — Returns the real current time when asked, calculated at runtime
- 📜 **Chat History Display** — Full conversation history is shown and refreshed after every message
- 🔄 **Clean Screen Refresh** — Uses `clear_output(wait=True)` for a smooth messenger-like experience
- 🚫 **Unknown Input Handling** — Responds helpfully when input is not recognized
- 👋 **Clean Exit** — Typing `bye`, `exit`, `quit`, or `goodbye` ends the chat gracefully
- 🧑 **Formatted Chat UI** — Clear visual separation between user and bot messages

---

## 🧠 Concepts Used

| Concept | Usage in This Project |
|---|---|
| `dictionary` | Maps keyword tuples to their corresponding responses |
| Tuple as dictionary key | Groups multiple keywords that mean the same thing |
| `any()` | Returns True if at least one keyword matches user input |
| `str.lower()` / `str.strip()` | Normalizes input so casing and spaces don't break matching |
| `datetime` | Gets real current time dynamically at runtime |
| `history` list | Stores full conversation for reprinting after each refresh |
| `clear_output()` | IPython function to refresh Jupyter cell output each round |
| f-strings | Clean, readable dynamic message formatting |
| Functions | Logic split into `get_response()`, `display_chat()`, `chatbot()` |

---

## 💬 Supported Commands

| What You Type | PyBot Responds With |
|---|---|
| `hello`, `hi`, `hey` | Greeting message |
| `how are you` | Status response |
| `name`, `who are you` | Bot introduction |
| `help`, `commands` | Lists available commands |
| `joke` | Tells a programming joke |
| `time`, `what time is it` | Current real time |
| `thanks`, `thank you` | Acknowledgement |
| `bye`, `exit`, `quit` | Ends the conversation |
| Anything else | Friendly fallback message |

---

## 📁 Project Structure

```
CodeAlpha_Chatbot/
│
├── chatbot.ipynb       # Main Jupyter Notebook — full chatbot code
├── README.md           # Project documentation (this file)
└── requirements.txt    # Python dependencies
```

---

## ⚙️ Requirements

- Python 3.x
- Jupyter Notebook or JupyterLab
- IPython (comes pre-installed with Jupyter)
- No external libraries needed

---

## 🚀 How to Run

**1. Clone the repository**
```bash
git clone https://github.com/hope-cs/CodeAlpha_Chatbot.git
cd CodeAlpha_Chatbot
```

**2. Launch Jupyter Notebook**
```bash
jupyter notebook chatbot.ipynb
```

**3. Start chatting**
- Open `chatbot.ipynb` in Jupyter
- Run all cells from top to bottom (`Cell → Run All`)
- The last cell starts the chatbot
- Type your message in the input box and press Enter

---

## 📸 Sample Output

```
=============================================
         🤖 PyBot — Python Chatbot
      Type 'bye' to exit the chat
=============================================

  🧑 You:   hello
  🤖 PyBot: 👋 Hello! How can I help you today?

  🧑 You:   time
  🤖 PyBot: 🕐 Current time is 10:50 AM

  🧑 You:   joke
  🤖 PyBot: 😄 Why do programmers prefer dark mode? Because light attracts bugs! 🐛

  🧑 You:   how are you
  🤖 PyBot: 😊 I'm doing great, thanks for asking! What about you?

  🧑 You:   bye
  🤖 PyBot: 👋 Goodbye! Have a great day!
```

---

## 🔧 Customization

You can easily extend PyBot by editing `chatbot.ipynb`:

- **Add new responses** → Add a new tuple-response pair to the `RESPONSES` dictionary in Cell 2
- **Add more keywords** → Extend any existing tuple with more trigger words
- **Add more dynamic responses** → Use the `"DYNAMIC_TIME"` placeholder pattern for responses that need runtime calculation (e.g. date, weather)

---

## 👨‍💻 Author

**Hamza Sajjad**
CodeAlpha Python Programming Intern
[GitHub Profile](https://github.com/hope-cs)

---

## 🏢 About CodeAlpha

CodeAlpha is a leading software development company providing internship programs focused on hands-on Python development experience.
[www.codealpha.tech](https://www.codealpha.tech)
