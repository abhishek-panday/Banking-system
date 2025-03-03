
# Python Bank Account Management System Condition

**Objective:**

Create a Python program that simulates a bank account management system. The system should allow users to create and manage bank accounts, perform transactions, and retrieve relevant details. The project should incorporate the key Python concepts you’ve learned, such as variables, data structures, functions, file handling, and modules.

# Requirements 

**Account Management:**

- Users should be able to create new bank accounts. Each account must have the following attributes:
    - Account holder's name
    - Account number (auto-generated)
    - Account type (e.g., savings or current)
    - Initial balance
- Allow users to retrieve account details, including account holder’s name, account number, account type, and current balance.

**Transactions:**

- Implement the following transactions:
    - Deposit: Users can deposit money into their accounts.
    - Withdrawal: Users can withdraw money, ensuring that the withdrawal does not exceed the current balance.
    - Transfer: Implement a function to transfer funds between two accounts.
    - Ensure that transactions update the account balance accordingly.

**File Handling:**

- Store account details and transaction history in files.
    - Implement functionality to read and write account data to a file (using the pickle library).
    - Load account data from the file at the start of the program and save updates to the file when the program terminates.
    - Ensure the program can append new transactions to the existing file without overwriting previous data.

**Reports:**

- Allow users to view transaction history for a specific account.
    - Show details like date, type of transaction (deposit, withdrawal, transfer), and amount.
- Generate summary statistics for each account, such as total deposits, total withdrawals, and average transaction amounts using NumPy functions.

**User Interaction:**
- Create an interactive menu to perform the following operations:
    - Open a new account
    - View account details
    - Perform transactions (deposit, withdraw, transfer)
    - View transaction history
    - Exit the program
- Use conditional statements and loops to ensure smooth navigation between different menu options.

**Error Handling:**
- Implement input validation (e.g., ensure deposit and withdrawal amounts are positive).
- Handle potential errors, such as attempting to withdraw more money than available in the account or transferring funds between non-existent accounts.