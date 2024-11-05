ATM System Program

This is a simple ATM simulation program written in C++. It allows users to interact with different types of bank accounts, such as savings, current, and premium accounts. The program supports basic banking operations such as checking balance, depositing money, withdrawing money, and adding interest to savings accounts. Premium accounts also have premium services.

Features:
Bank Account Management: Includes Savings, Current, and Premium accounts.


Operations:
Check balance
Deposit money
Withdraw money (with overdraft for current accounts)
Add interest to Savings accounts
Premium Account Services: Premium accounts have access to additional services.
ATM Simulation: Users can interact with accounts via an ATM interface, choose operations, and perform transactions.


Classes
Person: Represents a person with an ID and age.
BankAccount: Base class for bank accounts with methods for checking balance, depositing, and withdrawing money.
SavingsAccount: Inherits from BankAccount, adds interest rate functionality, and allows adding interest.
Overdraft: Provides functionality for overdraft protection, used by current accounts.
CurrentAccount: Inherits from BankAccount and Overdraft, allows withdrawal with overdraft protection.
PremiumAccount: Inherits from SavingsAccount, adds premium services.
ATM: Handles the ATM transactions for the user, displaying the menu, and performing operations based on user input.
Compilation and Execution



Requirements:
A C++ compiler (e.g., GCC or MSVC).
C++11 or later for features like nullptr, override, etc.
Steps to compile and run:
Save the source code in a .cpp file (e.g., atm_system.cpp).
Open a terminal or command prompt.
Navigate to the directory where the .cpp file is saved.
Compile the program using your preferred C++ compiler:
Using g++ (GCC):
bash
Copy code
g++ atm_system.cpp -o atm_system
Using cl (MSVC):
bash
Copy code
cl atm_system.cpp
Run the compiled program:
On Unix-like systems:
bash
Copy code
./atm_system
On Windows:
bash
Copy code
atm_system.exe
Program Workflow


Login: The user is prompted to enter an account number.
Account Selection: The user selects the type of account (Savings, Current, or Premium).
ATM Operations:
The ATM menu allows the user to:
Check balance
Deposit funds
Withdraw funds (with overdraft for current accounts)
Add interest (only for Savings accounts)
Exit or return to the main menu
Premium Account: If the user selects a Premium account, premium services are provided.
The user can continue performing transactions until they choose to exit.

Sample Output
mathematica
Copy code
Welcome to the ATM System
Enter account number: 101
Select account type:
1. Savings Account
2. Current Account
3. Premium Account
Choose account type: 1

ATM Menu:
1. Check Balance
2. Deposit
3. Withdraw
4. Add Interest
5. Exit
6. Return to Main Menu
Choose an option: 4
Interest added. New balance: $1025.000
Do you want to perform another transaction? (Y/N): N
Thank you for using the ATM System. Goodbye!
Future Enhancements
File-based Account Management: Save and load accounts from a file (e.g., CSV or JSON).
Account Validation: Implement password protection or PIN verification for secure access to accounts.
Transaction History: Keep a record of transactions (deposits, withdrawals) for each account.
Multiple Users: Support for multiple users with different account types.
