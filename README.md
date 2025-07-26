🏦 Bank Management System (Mini Project in C)

**🎯 Objective**
- To simulate a real-time banking system that supports:
- Account creation
- Transactions (Deposit, Withdraw, Transfer)
- Balance enquiry
- Transaction history (last 5)
- Persistent data storage
- Account search and listing

**🧠 Key Features**
- Each account holds:
    - Account number
    - Holder’s name
    - Contact number
    - Balance
    - Linked list of transactions
- Transactions track:
    - Type (Deposit, Withdraw)
    - Unique transaction ID
    - Amount
- Persistent data storage via accounts.dat file
- Menu-driven interface
- Supports Single Linked List (SLL) for accounts and transactions
- Prevents duplicate account numbers

**🧾 Menu Interface**
When the app runs, it shows:
------------------MENU---------------------------
C/c: Create account
H/h: Transaction history (minimum last 5)
W/w: Withdraw amount
D/d: Deposit amount
B/b: Balance enquiry
T/t: Transfer money
E/e: Display all accounts
S/s: Save accounts info
F/f: Find account
Q/q: Quit

**🧪 Functional Breakdown**
**✅ Create Account**
-  User provides unique account number, name, and contact
-  Initializes with 0 balance
-  Checks for duplicate account number

**💸 Deposit / Withdraw**
-  Modifies balance
-  Logs transaction in linked list
-  Withdraw checks for sufficient balance

**🔁 Transfer**
-  Transfers amount from one account to another
-  Logs transactions in both accounts

**📄 Transaction History**
-  Displays last 5 transactions using linked list traversal

**🔍 Search Account**
-  Search by account number
-  Shows name, balance, and contact

**🧾 Display All Accounts**
-  Lists all registered accounts with brief details

**💾 Save/Load Data**
-  Uses binary file accounts.dat for persistent storage
-  On start, load_data() restores data
-  On exit or manual save, save_data() writes to file

** � Notes**
-  Make sure account_number is unique
-  Handles input validation and basic error checking
-  Implemented using user-defined functions for modularity

