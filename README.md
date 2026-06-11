# 📝 User Memory Saver Agent

A simple Python-based Memory Agent that continuously stores user inputs into a text file along with timestamps. The agent creates a persistent memory log that can be used to track user interactions over time.

This project demonstrates the fundamentals of memory systems used in AI agents and chatbots.

---

# 📌 Project Overview

Most chatbots forget information once the session ends.

This Memory Saver Agent solves that problem by:

* Capturing user input
* Recording the current timestamp
* Saving data permanently into a text file
* Maintaining a historical memory log

This project is useful for understanding how memory works in AI systems.

---

# 🚀 Features

✅ Stores user messages permanently

✅ Adds timestamp to every entry

✅ Creates persistent memory

✅ Works offline

✅ Lightweight and fast

✅ Beginner-friendly project

✅ Compatible with Google Colab and Jupyter Notebook

---

# 🛠️ Technologies Used

| Technology    | Purpose                   |
| ------------- | ------------------------- |
| Python        | Programming Language      |
| datetime      | Generate timestamps       |
| File Handling | Store user data           |
| Text Files    | Persistent memory storage |

---

# 📂 Project Structure

```text
user-memory-agent/
│
├── app.py
├── user_memory.txt
├── requirements.txt
└── README.md
```

---

# ⚙️ Installation

No external libraries are required.

Python built-in modules are sufficient.

Check Python version:

```bash
python --version
```

---

# ▶️ Run The Project

```bash
python app.py
```

---

# 💻 Source Code

```python
from datetime import datetime

FILE_NAME = "user_memory.txt"

print("📝 User Memory Saver")
print("Type 'exit' to stop\n")

while True:

    user = input("You: ")

    if user.lower() == "exit":
        break

    timestamp = datetime.now().strftime(
        "%Y-%m-%d %H:%M:%S"
    )

    with open(
        FILE_NAME,
        "a",
        encoding="utf-8"
    ) as f:

        f.write(
            f"[{timestamp}] {user}\n"
        )

    print("✅ Saved")
```

---

# 🔍 Complete Code Explanation

## Import datetime

```python
from datetime import datetime
```

### Purpose

Imports the datetime module used to generate timestamps.

Example:

```python
datetime.now()
```

Output:

```text
2026-06-11 15:30:45
```

---

## Define Memory File

```python
FILE_NAME = "user_memory.txt"
```

### Purpose

Specifies the file where user memories will be stored.

---

## Welcome Message

```python
print("📝 User Memory Saver")
```

### Purpose

Displays the project title when the program starts.

---

## Infinite Loop

```python
while True:
```

### Purpose

Keeps the program running continuously until the user exits.

---

## User Input

```python
user = input("You: ")
```

### Purpose

Accepts text from the user.

Example:

```text
My name is Ajay
```

---

## Exit Condition

```python
if user.lower() == "exit":
    break
```

### Purpose

Stops the program safely when the user types:

```text
exit
```

---

## Generate Timestamp

```python
timestamp = datetime.now().strftime(
    "%Y-%m-%d %H:%M:%S"
)
```

### Purpose

Generates the current date and time.

Example:

```text
2026-06-11 15:45:12
```

---

## Save Data to File

```python
with open(
    FILE_NAME,
    "a",
    encoding="utf-8"
) as f:
```

### Purpose

Opens the memory file in append mode.

Append mode ensures previous data remains intact.

---

## Write Memory Entry

```python
f.write(
    f"[{timestamp}] {user}\n"
)
```

### Purpose

Stores user input with timestamp.

Example:

```text
[2026-06-11 15:45:12] My name is Ajay
```

---

# 🔄 Project Workflow

```text
User Input
     │
     ▼
Generate Timestamp
     │
     ▼
Open Memory File
     │
     ▼
Store Data
     │
     ▼
Save Memory
```

---

# 📊 Example

## Input

```text
You: My name is Ajay
You: I am learning AI
You: Python is awesome
```

---

## Generated File

```text
[2026-06-11 15:30:10] My name is Ajay
[2026-06-11 15:30:22] I am learning AI
[2026-06-11 15:30:40] Python is awesome
```

---

# 🎯 Applications

* Personal Memory Tracking
* AI Agent Memory Systems
* User Activity Logging
* Chat History Storage
* Research Data Collection
* Learning Agent Development

---

# Advantages

* Simple and Easy to Understand
* Persistent Storage
* Lightweight
* No External Dependencies
* Works Offline
* Easy to Extend

---

# Limitations

* Stores Only User Messages
* No Search Functionality
* No Database Integration
* No Memory Categorization

---

# Future Improvements

* Search Stored Memories
* Filter by Date
* Export to CSV
* Export to PDF
* SQLite Database Integration
* Memory Retrieval System
* AI-Based Memory Summarization
* Streamlit Dashboard

---

# Learning Outcomes

After completing this project, you will understand:

* Python File Handling
* Timestamp Generation
* Persistent Storage
* Basic Agent Memory Systems
* User Data Logging
* Program Loops and Conditions

---

# Resume Description

Developed a User Memory Saver Agent using Python that records user inputs with timestamps and stores them in a persistent text file. The system demonstrates the core concepts of memory management and data persistence used in AI agents.

---

# 👨‍💻 Author

## Ajay Sagar

* Python Developer
* AI & Machine Learning Enthusiast
* B.Tech CSE Student

### Connect With Me

🔗 LinkedIn: https://www.linkedin.com/in/engineerajay

🚀 Building AI Projects and Learning New Technologies Every Day.

**Code the Future with Us..!**
