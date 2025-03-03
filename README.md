# Banking-system
# Key Components of the Code
**Account Class:**

Represents a bank account with attributes like name, account_number, account_type, balance, and transactions.

**Methods include:**

- **_deposit():_** Adds funds to the account.

- **_withdraw():_** Deducts funds from the account.

- **_transfer():_** Transfers funds to another account.

- **_get_transaction_history():_** Returns the list of transactions.

- **_get_summary_statistics():_** Provides summary statistics (total deposits, withdrawals, and average transaction amount).

- **_view_passbook():_** Displays a formatted passbook with transaction history.

- **_generate_account_number():_** Generates a unique 10-digit account number.

**File Handling:**

The program uses the pickle module to save and load account and transaction data to/from files (accounts.pkl and transactions.pkl).

- **_load_data():_** Loads existing accounts and transactions from files.

- **_save_data():_** Saves the current state of accounts and transactions to files.

- **Main Program:**

Provides a menu-driven interface for users to interact with the system.

**Options include:**

- Open a new account.

- View account details.

- Perform transactions (deposit, withdraw, transfer).

- View transaction history.

- View passbook.

- Exit the program and save data.

# Significance of the Code
**Object-Oriented Design:**

The Account class encapsulates all the properties and behaviors of a bank account, making the code modular and reusable.

This design allows for easy extension, such as adding new account types or transaction types.

**Data Persistence:**

By using pickle, the program can save and load data between sessions, ensuring that account and transaction data are not lost when the program exits.

**User-Friendly Interface:**

The menu-driven interface makes it easy for users to interact with the system without needing to understand the underlying code.

**Transaction Tracking:**

Every transaction (deposit, withdrawal, transfer) is recorded with a timestamp, allowing users to view a detailed history of their account activity.

**Error Handling:**

The program includes basic checks to prevent invalid transactions (e.g., withdrawing more than the available balance or transferring to a non-existent account).

**Unique Account Number Generation:**

The generate_account_number() method ensures that each account has a unique 10-digit number, which is essential for identifying accounts in a real-world banking system.

**How It Works**
**Initialization:**

When the program starts, it loads existing accounts and transactions from the pickle files.

- _Menu Options:_

Users can choose from various options to manage their accounts:

- _Open a new account:_ Creates a new Account object and adds it to the accounts dictionary.

- _View account details:_ Displays the account holder's name, account number, type, and balance.

- _Perform transactions:_ Allows users to deposit, withdraw, or transfer funds.

- _View transaction history:_ Displays a list of all transactions for a specific account.

- _View passbook:_ Shows a formatted passbook with transaction details and running balances.

- _Exit:_ Saves the current state of accounts and transactions to files and exits the program.

**Data Persistence:**

When the program exits, it saves the current state of accounts and transactions to the pickle files, ensuring that data is preserved for future sessions.

Example Usage
**_Open a New Account:_**

User provides their name, account type, and initial balance.

The program generates a unique account number and creates a new Account object.

**_Deposit Funds:_**

User selects the deposit option and enters the amount.

The program updates the account balance and records the transaction.

**_View Passbook:_**

User selects the passbook option and enters their account number.

The program displays a formatted passbook with transaction history and running balances.

**_Exit:_**

User selects the exit option, and the program saves all data to the pickle files before terminating.
