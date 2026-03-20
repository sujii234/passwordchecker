# passwordchecker


📌 Overview

This project is a simple Python-based password strength checker that evaluates a user's password using multiple security criteria such as length, character types, and complexity.

It provides:

Strength rating (Weak / Medium / Strong)

Suggestions to improve weak passwords

⚙️ Features

Checks minimum password length

Validates:

Uppercase letters

Lowercase letters

Numbers

Special characters

Gives improvement suggestions

Simple and beginner-friendly logic

🛠️ Requirements

Python 3.x

Built-in module: re (Regular Expressions)

🚀 How to Run

Save the file as:

Python password check.py

Open terminal / command prompt

Run:

python "Python password check.py"
🧠 How It Works (Process)
1. Input Password
password = input("Enter your password: ")

Takes user input from terminal

2. Initialize Score System
score = 0
suggestions = []

Score determines strength

Suggestions list stores improvements

3. Validation Checks
✔ Length Check

Minimum 8 characters required

✔ Uppercase Check

Uses regex: [A-Z]

✔ Lowercase Check

Uses regex: [a-z]

✔ Digit Check

Uses regex: \\d

✔ Special Character Check

Uses regex: [!@#$%^&*(),.?":{}|<>]

👉 Process:

Each valid condition increases score

Failed condition adds a suggestion

4. Strength Classification
if score <= 2:
    strength = "Weak ❌"
elif score == 3 or score == 4:
    strength = "Medium ⚠️"
else:
    strength = "Strong ✅"

👉 Logic:

0–2 → Weak

3–4 → Medium

5 → Strong

5. Output Result

Displays password strength

Shows suggestions if needed

💬 Example Output
Enter your password: hello123

Password Strength: Medium ⚠️
Suggestions to improve:
- Add uppercase letters
- Add special characters
⚡ Key Concepts Used

Regular Expressions (re)

Conditional Logic

Functions

Input/Output Handling

🔐 Security Note

This is a basic checker and does NOT:

Encrypt passwords

Store passwords securely

Protect against real-world attacks

Use it for learning purposes only.

🔮 Future Improvements

Add password entropy calculation

Integrate with GUI (Tkinter / Web app)

Add real-time strength meter

Store hashed passwords securely

API integration for breached password check

📄 License

Free to use for educational and personal projects.
