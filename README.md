# 💰 Mini Banking System

A simple Python-based mini banking system that allows users to create accounts, deposit and withdraw funds, check balances, and view transaction history. The system also supports automated software testing using `pytest`.

---

## 📌 Project Description

The **Mini Banking System** is designed to simulate basic banking functionalities in a lightweight environment. This system is suitable for learning software development, testing, and small-scale simulation of banking operations. It includes user account management, transaction logging, and basic validations.

---

## ✅ Features

- Account creation with name and initial deposit
- Secure deposit and withdrawal of funds
- Balance inquiry at any time
- Transaction history logging
- Account closure
- Admin panel to view all accounts (optional)
- CLI interface (GUI/Flask optional for enhancement)

---

## 🔧 Functional Requirements

| Feature | Description |
|---------|-------------|
| **Account Creation** | Users can open an account with name, ID, and initial deposit. |
| **Login/Authentication** | User must log in using ID and password (optional). |
| **Deposit Money** | Users can deposit money into their account. |
| **Withdraw Money** | Users can withdraw money, given sufficient balance. |
| **Balance Inquiry** | Users can check current balance. |
| **Transaction History** | All transactions are logged and viewable. |
| **Close Account** | Users or admin can delete an account. |
| **Admin Panel** | (Optional) View all users and account data. |

---

## ⚙️ Non-Functional Requirements

- **Security**: Secure handling of user data and inputs.
- **Performance**: Efficient handling of multiple transactions.
- **Scalability**: Modular design for future extensions.
- **Usability**: Command-line user interface (CLI).
- **Testability**: Fully testable with automated unit tests.

---

## 🧪 Software Testing Plan

The project includes a robust test suite using `pytest`.

| Test Type | Target | Example |
|-----------|--------|---------|
| Unit Testing | Functions like `deposit()`, `withdraw()` | Ensure correct amount added or subtracted |
| Integration Testing | Account + Deposit + Withdraw | Check balance after a series of operations |
| Boundary Testing | Edge input values | Withdraw exactly the available balance |
| Negative Testing | Invalid inputs | Deposit negative value or withdraw more than balance |
| Performance Testing (Optional) | Simulate bulk transactions | Track system behavior under load |
| Security Testing (Optional) | Access control | Ensure unauthorized actions are prevented |

---

## 🏗️ Project Structure
mini-banking-system/
├── bank.py # Core logic (BankAccount class)
├── test_bank.py # Pytest unit test cases
├── main.py # Optional CLI interface
├── README.md # Project documentation
