# 🔍 Code Analyzer for Beginners

A beginner-friendly web app that analyzes, runs, and explains code token-by-token. Paste your code, select a language, and get syntax highlighting, live output, and a plain-English explanation of every keyword, operator, and symbol.

---

## 🚀 Features

- 📝 **Code Input** — Paste code directly with optional user inputs for interactive programs
- ▶️ **Code Execution** — Compiles and runs the submitted code in real time
- 🎨 **Syntax Highlighting** — Color-coded code rendering with line numbers via Pygments
- 🔑 **Token Explanation** — Breaks code into tokens and explains each one in plain English (keywords, operators, data types, functions, symbols, etc.)
- ❌ **Error Handling** — Displays syntax errors and runtime/compilation errors clearly

---

## 🛠️ Supported Languages

| Language | Run | Syntax Check | Token Explanation |
|---|---|---|---|
| Python | ✅ | ✅ (ast) | ✅ |
| C | ✅ (gcc) | ✅ | ✅ |
| C++ | ✅ (g++) | ✅ | ✅ |
| Java | ✅ (javac/java) | ✅ | ✅ |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Code Execution | subprocess (gcc, g++, javac, python3) |
| Syntax Highlighting | Pygments |
| Syntax Validation | Python `ast` module |
| Frontend | HTML, CSS (Jinja2 templates) |

---

## ⚙️ Setup

1. **Clone the repository.**

2. **Install dependencies:**
```bash
   pip install flask pygments
```

3. **Ensure compilers are installed and available in PATH:**
   - Python 3
   - GCC (for C)
   - G++ (for C++)
   - JDK (for Java — `javac` and `java`)

4. **Run the app:**
```bash
   python app.py
```

5. **Open in browser:**
http://127.0.0.1:5000

---

## 📁 Project Structure
Code-Analyzer-for-Beginners/
├── app.py # Flask app — routing, execution, analysis logic
├── token_explainer.py # Token-to-explanation mapping for all languages
├── templates/
│ ├── index.html # Code input form
│ ├── result.html # Analysis results with highlighted code and token table
│ └── error.html # Error display page
└── syntax.html # Static syntax reference page

---

## 📄 License

This project is for educational purposes.
