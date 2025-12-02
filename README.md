# Simple-banking-system-sem-3
This model helps the users to manage their banking easier
Simple Banking System

Project Overview

This is a console-based application developed in Java that simulates fundamental banking operations. The system allows users to create accounts, deposit funds, withdraw funds, check account balances, and view a list of all registered accounts. It's designed with a focus on clean code, proper error handling, and modularity, adhering to standard software development best practices.
Core Features

Account Creation: Create new bank accounts with a unique account number, account holder's name, and an initial balance.
Deposit Funds: Add money to an existing account.
Withdraw Funds: Remove money from an existing account, with checks for sufficient balance.
Check Balance: View the current balance of a specific account.
List All Accounts: Display details for all accounts currently in the system.

Getting Started

Prerequisites
Java Development Kit (JDK) 8 or higher installed on your system.

Installation and Setup
Clone the Repository:
git clone <your-github-repo-link-here>
cd SimpleBankingSystem

(Note: Replace <your-github-repo-link-here> with the actual URL of your GitHub repository once uploaded.)
Save Files:
Ensure you have the following Java files in your project directory (e.g., in a src folder or directly in the root):
InsufficientFundsException.java
Account.java
Bank.java
BankingApp.java
Compile the Code:
Open your terminal or command prompt, navigate to the directory where your .java files are located, and compile them:
javac InsufficientFundsException.java Account.java Bank.java BankingApp.java


Run the Application:
After successful compilation, run the main application:
java BankingApp



Usage

Once the application is running, you'll see a console menu. Enter the number corresponding to the operation you wish to perform and follow the on-screen prompts.
--- Simple Banking System Menu ---
1. Create Account
2. Deposit Funds
3. Withdraw Funds
4. Check Balance
5. List All Accounts
6. Exit
Enter your choice:



Example Workflow:

Create Account: Choose 1, enter holder name and initial balance.
Deposit: Choose 2, enter account number and amount.
Withdraw: Choose 3, enter account number and amount.
Check Balance: Choose 4, enter account number.
List Accounts: Choose 5.
Exit: Choose 6 to quit the application.

Project Structure

The project is organized into distinct classes, following Object-Oriented Programming (OOP) principles:
InsufficientFundsException.java: A custom exception class for handling insufficient balance scenarios.
Account.java: Represents a single bank account, managing its balance and providing deposit/withdrawal functionalities.
Bank.java: Acts as the central manager for all accounts, handling account creation, retrieval, and transaction delegation.
BankingApp.java: Contains the main method and provides the console-based user interface for interacting with the bank system.

Error Handling and Robustness

The system incorporates robust error handling to prevent crashes and ensure data integrity:
Custom Exceptions: InsufficientFundsException is used for balance-related errors during withdrawals.
Input Validation: Checks are in place for positive amounts (deposits, withdrawals) and sufficient funds.
Input Mismatch Handling: Uses try-catch blocks with InputMismatchException to handle non-numeric user inputs gracefully.
Account Existence Check: Validates if an entered account number exists before proceeding with transactions.

Future Enhancements

Transaction History: Implement logging of all transactions (deposits, withdrawals) for each account.
Account Types: Introduce different account types (e.g., Savings, Checking) with specific rules or features (e.g., interest rates).
User Authentication: Add a basic login system for account holders.
Persistence: Integrate with a database (e.g., SQLite, MySQL) or file system to save account data permanently, instead of losing it when the application closes.
Graphical User Interface (GUI): Develop a GUI using JavaFX or Swing for a more user-friendly experience.
