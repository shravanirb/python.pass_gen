# 🔐 Smart Password Generator Using Personal Questions

## 📌 Project Overview

The **Smart Password Generator** is a Python-based application designed to generate strong and secure passwords using randomly selected personal questions. The system uses answers related to users' daily routines, favourite things, personal preferences, and interests to create personalized passwords.

It automatically ensures that generated passwords meet essential security requirements, checks their strength, and provides an option to save generated passwords locally or to Google Sheets.

## 🎯 Project Objectives

- Generate strong and random passwords.
- Allow users to select their desired password length.
- Use personal questions to create personalized passwords.
- Ensure passwords contain uppercase letters, lowercase letters, numbers, and special characters.
- Evaluate password strength automatically.
- Store generated passwords with their generation date and strength.
- Provide optional Google Sheets integration for cloud storage.

## ✨ Key Features

### 1. Random Personal Question Selection
- Contains a predefined bank of 80 personal questions.
- Questions are based on daily life, hobbies, family, education, favourite things, and personal interests.
- Randomly selects 3 questions each time the program runs.
- Uses user answers as part of password generation.

### 2. Strong Password Generation

The generated password follows these security requirements:

| Requirement | Description |
|---|---|
| Uppercase | At least one capital letter (A–Z) |
| Lowercase | At least one small letter (a–z) |
| Number | At least one digit (0–9) |
| Special Character | At least one symbol (@, #, $, etc.) |
| Minimum Length | 8 characters |

Users can also select their desired password length.

### 3. Password Strength Checker

The application automatically evaluates the generated password based on five conditions:

- Uppercase letters
- Lowercase letters
- Numbers
- Special characters
- Minimum password length

It displays one of three strength levels:

- Weak
- Medium
- Strong

### 4. Local Password Storage

Generated passwords are automatically saved in a text file named `generated_passwords.txt`.

The file stores:
- Date and time
- Generated password
- Password strength

### 5. Google Sheets Integration (Optional)

The project supports Google Sheets integration using:
- `gspread`
- `oauth2client`

It can save generated passwords and their strength information to a Google Sheet.

## 🛠️ Technologies & Libraries Used

**Programming Language:** Python

**Python Libraries:**

| Library | Purpose |
|---|---|
| `random` | Random question and character selection |
| `string` | Uppercase, lowercase, digits, and symbols |
| `datetime` | Recording date and time |
| `gspread` | Google Sheets integration |
| `oauth2client` | Google API authentication |
| `PyInstaller` | Converting Python code into an executable |

## 📂 Project Structure

```text
SmartPasswordGenerator/
│
├── smart_password_generator.py
├── generated_passwords.txt
├── credentials.json       (Optional)
├── README.md
└── requirements.txt       (Optional)
```

## ⚙️ Installation & Setup

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

### Step 2: Open the Project Folder

```bash
cd SmartPasswordGenerator
```

### Step 3: Run the Python Program

```bash
python smart_password_generator.py
```

### Step 4: Install Optional Google Sheets Libraries

```bash
python -m pip install gspread oauth2client
```

## ▶️ How to Use

1. Run the Python program.
2. Enter your desired password length (minimum 8 characters).
3. Answer the 3 randomly selected personal questions.
4. The system generates a password using your answers and random characters.
5. View your generated password.
6. Check the displayed password strength.
7. The password is saved locally in a text file.
8. If Google Sheets is configured, the password is also saved online.

## 💻 Sample Output

```text
=================================
     SMART PASSWORD GENERATOR
=================================

Enter desired password length: 12

Answer the following questions:

What is your favorite food? Pizza
What is your favorite color? Blue
What is your favorite hobby? Reading

Generated Password: Example@7Ab12

Password Strength: Strong

Saved to Google Sheet

Password saved successfully.
```

*Note: The sample output is illustrative.*

## 📦 Convert Python Project into EXE

The project can be converted into a Windows executable using PyInstaller.

Install PyInstaller:

```bash
python -m pip install pyinstaller
```

Generate the executable:

```bash
python -m PyInstaller --onefile smart_password_generator.py
```

The executable will be available inside the `dist` folder.

## 🚀 Future Enhancements

- Develop a professional GUI using Tkinter.
- Add a password history viewer.
- Introduce password encryption.
- Add an option to generate multiple passwords.
- Improve password randomness and security.
- Integrate a secure cloud-based password manager.

## ⚠️ Security Note

This project is developed for educational and demonstration purposes.

- Personal questions and answers should not be treated as security secrets.
- Avoid using real names, birthdays, family details, or other predictable personal information in actual passwords.
- Python's `random` module is not cryptographically secure. A production password generator should use Python's `secrets` module.
- Do not upload `credentials.json` or real passwords to GitHub.
- Never commit generated password history files containing actual passwords.
- Use secure storage and encryption for real-world password management.

## 🎓 Project Information

**Project Name:** Smart Password Generator Using Personal Questions

**Domain:** Python Programming / Cybersecurity

**Project Type:** College Mini Project

**Developed By:** Shravani Birajdar

**Language:** Python

---

## ⭐ Conclusion

The Smart Password Generator demonstrates how Python can be used to develop a personalized password generation system. By combining random question selection, password generation, strength evaluation, and optional Google Sheets integration, the project provides an educational implementation of password security concepts.

**If you find this project interesting, don't forget to give it a ⭐!**
