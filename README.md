##Personal Account Management

Overview

This Java project provides a class called PersonalAccount for personal bank account management. It allows users to create and manage their accounts by performing operations such as depositing, withdrawing, checking balances, and viewing transaction history.

Contents

Project Structure
Class Structure
Usage
Testing
GitHub Repository
Contributors
License
Project Structure

The project consists of two main Java classes:

PersonalAccount: Represents a personal bank account, with methods for depositing, withdrawing, checking balances, and viewing transaction history.
Amount: Represents a transaction amount, with an amount value and a transaction type.
Class Structure

PersonalAccount
The PersonalAccount class has the following instance variables:

accountNumber (int): A unique identifier for the account.
accountHolder (String): The name of the account holder.
balance (double): The current balance in the account.
transactions (an array of "Amount" objects): An array to store deposit and withdrawal transactions.
The methods include:

PersonalAccount(int accountNumber, String accountHolder): A constructor to initialize the account with a unique account number, account holder's name, and an initial balance of 0.0.
void deposit(double amount): Deposits money into the account, adds the deposit transaction to the transactions array, and updates the balance.
void withdraw(double amount): Withdraws money from the account, adds the withdrawal transaction to the transactions array, and updates the balance. Ensures that the withdrawal amount does not exceed the current balance.
void printTransactionHistory(): Prints the transaction history (all transactions) of the account, including transaction type and amount.
double getBalance(): Retrieves the current balance of the account.
int getAccountNumber(): Retrieves the account number.
String getAccountHolder(): Retrieves the account holder's name.
Amount
The Amount class represents a transaction amount and includes:

amount (double): The transaction amount.
transactionType (String): A string indicating the type of transaction (e.g., "Deposit" or "Withdrawal").

