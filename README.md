# 🏧 ATM Management System

A simple **ATM Management System built using Python**. This beginner-friendly project demonstrates the use of dictionaries, loops, conditional statements, user input, functions of an ATM, and transaction history.

## 📌 Project Overview

This project simulates basic ATM operations. The user must enter a valid **4-digit ATM PIN** to access the ATM services.

After successful authentication, the user can:

* 💸 Withdraw money
* 💰 Deposit money
* 💳 Check account balance
* 🔐 Change ATM PIN
* 📜 View transaction history
* 🚪 Exit the ATM

The system also provides **3 PIN attempts**. After three incorrect attempts, the card is temporarily blocked.

---

## ✨ Features

### 🔐 PIN Authentication

* User enters their ATM PIN.
* PIN must contain exactly 4 characters.
* User gets a maximum of **3 attempts**.
* After 3 incorrect attempts, the card is temporarily blocked.

### 💸 Withdraw Money

The withdrawal feature:

* Checks whether sufficient balance is available.
* Accepts withdrawal amounts only in multiples of ₹100.
* Deducts the withdrawn amount from the account balance.
* Stores the withdrawal in transaction history.

### 💰 Deposit Money

The deposit feature:

* Accepts deposit amounts only in multiples of ₹100.
* Adds the deposited amount to the account balance.
* Stores the deposit in transaction history.

### 💳 Balance Check

Displays the user's current account balance.

### 🔐 PIN Change

The user can change their ATM PIN by:

1. Entering the existing PIN.
2. Entering a new 4-digit PIN.
3. Updating the ATM PIN.

### 📜 Transaction History

The system stores transactions in a list and displays them when requested.

Example:

```text
withdead amount:1000
Deposit amount:5000
```

---

## 🛠️ Technologies Used

* **Python 3**
* Python Dictionary
* Python List
* `while` loop
* `if-elif` conditional statements
* `input()` function
* f-strings
* String operations
* Basic exception-free console interaction

---

## 📂 Project Structure

```text
ATM-Management-System/
│
├── atm.py
└── README.md
```

### `atm.py`

Contains the complete Python source code for the ATM Management System.

### `README.md`

Contains the project documentation, features, setup instructions, and usage information.

---

## ⚙️ Requirements

You only need:

* Python 3.x

No external Python libraries are required.

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/ATM-Management-System.git
```

### 2. Open the Project Folder

```bash
cd ATM-Management-System
```

### 3. Run the Python Program

```bash
python atm.py
```

On some systems, you may need:

```bash
python3 atm.py
```

---

## 🔑 Default ATM Details

The program currently contains the following sample account information:

```text
Name       : rocky
ATM PIN    : 3530
Balance    : ₹500000
```

> ⚠️ **Note:** This is only a practice project. Never store a real ATM PIN, bank account information, or other sensitive credentials directly inside source code.

---

## 🖥️ Example Usage

When the program starts:

```text
welcome to the ATM
enter your pin: 3530
```

After entering the correct PIN:

```text
enter
1.withdraw
2.deposit
3.balance
4.pin change
5.Transaction History
Enter your option:
```

### Example: Check Balance

```text
Enter your option: 3

your current balance was 500000

1.home
2.exit
Enter your option:
```

### Example: Withdraw

```text
Enter your option: 1
enter withdraw amount:1000

you drawed 1000 and your balance was 499000
```

### Example: Deposit

```text
Enter your option: 2
enter deposit amount:5000

you have deposited 5000 your current balance was 504000
```

### Example: Transaction History

```text
Enter your option: 5

withdead amount:1000
Deposit amount:5000
```

---

## 🔒 PIN Attempt System

The ATM allows a maximum of **3 incorrect PIN attempts**.

Example:

```text
enter your pin: 1234
you entered invalid pin remaining attempts are 2

enter your pin: 1111
you entered invalid pin remaining attempts are 1

enter your pin: 2222
your card was temporarly blocked
```

---

## 📚 Python Concepts Demonstrated

This project is useful for practicing the following Python concepts:

### Dictionary

```python
details_ = {
    "name": "rocky",
    "ATM PIN": "3530",
    "balance": 500000,
    "Transaction": []
}
```

### While Loop

```python
while remaining_atmp > 0:
    ...
```

### Conditional Statements

```python
if user_inp == 1:
    ...
elif user_inp == 2:
    ...
```

### List

```python
details_["Transaction"].append("Deposit amount:5000")
```

### String Formatting

```python
print(f"your current balance was {details_['balance']}")
```

### User Input

```python
pin = input("enter your pin:")
```

---

## 🔮 Future Improvements

The project can be improved by adding:

* [ ] Multiple bank accounts/users
* [ ] Account number authentication
* [ ] PIN encryption
* [ ] Transfer money between accounts
* [ ] Mini statement
* [ ] Daily withdrawal limit
* [ ] Deposit validation
* [ ] Better error handling using `try-except`
* [ ] Proper `elif` structure
* [ ] Functions for each ATM operation
* [ ] Object-Oriented Programming (OOP)
* [ ] Database integration using MySQL
* [ ] GUI using Tkinter
* [ ] Web-based ATM application
* [ ] Persistent transaction history

---

## ⚠️ Important Note

This project is created for **educational and practice purposes only**.

It is **not a real banking application** and should not be used with actual financial information or credentials.

---

## 👨‍💻 Author

**Rocky**

Python Beginner / Full Stack Developer

---

## ⭐ Contributing

Suggestions and improvements are welcome.

If you would like to improve this project:

1. Fork the repository.
2. Create a new branch.
3. Make your changes.
4. Commit your changes.
5. Create a Pull Request.

---

## 📄 License

This project is intended for educational purposes.
