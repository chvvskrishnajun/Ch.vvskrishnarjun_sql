Banking Management System
=========================

*Project Overview:
-----------------
The Banking Management System is a college-level SQL project built using **MySQL 8.0 or later**. It stores and retrieves information about bank branches, customers, employees, accounts, transactions, and transfers.

*Note: This is an educational demo using fictional records. Do not use it with real customer or financial data.
------

*Objectives:
-----------
- Organize banking information in relational tables.
- Connect customers and accounts with their respective branches.
- Store account transactions and transfer history.
- Run SQL queries to retrieve account details, balances, transaction records, and summary reports.

* Technologies Used:
--------------------
- Database: MySQL 8.0+
- Language: SQL

*Database Setup:
----------------
1. Open MySQL Workbench or another MySQL 8.0+ client.
2. Open `Banking_Management_System.sql`.
3. Execute the script.
4. The script creates and selects the `banking_management` database, creates the tables, and inserts fictional demo records.
5. Run the example `SELECT` queries at the end of the script to view sample reports.

*Important: The script begins with `DROP DATABASE IF EXISTS banking_management;`. Running it again deletes and recreates that database, including 
------------its existing data. Back up any important data before execution.

*Database Tables:
----------------
| Table | Purpose |
|---|---|
| `branches` | Stores branch name, IFSC code, and city. |
| `customers` | Stores customer name, phone, email, address, and creation time. |
| `employees` | Stores employee details and the branch where each employee works. |
| `accounts` | Stores account number, owner, branch, type, balance, status, and opening date. |
| `transactions` | Stores deposits, withdrawals, transfer-in/out records, amounts, and transaction timestamps. |
| `transfers` | Stores source and destination accounts, transfer amount, status, time, and reference note. |

*Relationships:
--------------
- One branch can have many employees.
- One branch can have many accounts.
- One customer can have multiple accounts.
- One account can have many transaction records.
- A transfer links a source account and a destination account.

*SQL Features Demonstrated:
---------------------------
- `CREATE DATABASE` and `CREATE TABLE`
- Primary keys, foreign keys, unique constraints, and check constraints
- `INSERT` statements with fictional sample data
- `SELECT`, `WHERE`, `ORDER BY`, and `LIKE`
- `INNER JOIN` and `LEFT JOIN`
- Aggregate functions such as `COUNT()` and `SUM()`
- `GROUP BY`
- `CASE` expressions
- `UNION ALL`
- Indexes on transaction time and account ID

*Example Reports Included:
--------------------------
The SQL script includes queries to:
1. List accounts with customer and branch details.
2. Find active accounts with balances above 10,000.
3. Show transaction history for a specified account.
4. Summarize account counts and balances by branch.
5. Count accounts held by each customer.
6. Display transfer history with source and destination account numbers.
7. Calculate recorded deposits and withdrawals per account.
8. Search for customers whose names contain `Rao`.
9. Count records in each project table using `UNION ALL`.

* Limitations:
--------------
- This is a demonstration database, not a production banking application.
- The sample data is fictional.
- The SQL script records transactions and transfers, but it does not implement a complete, secure banking transaction workflow.
- No user authentication, authorization, encryption, or production-grade audit controls are included.

Future Enhancements – Banking Management System:
-----------------------------------------------
1. Online Banking: Develop a website or mobile application that allows customers to access their accounts online.
   --------------
2. Secure Login System: Add usernames, passwords, and role-based access for customers, employees, and administrators.
   --------------------
3. Money Transfer: Improve the existing transfers table to support secure transfers between accounts with proper balance validation.
   --------------
4. Loan Management: Add a loan module to manage loan applications, approvals, repayments, and interest rates.
   ---------------
5. ATM Management: Add ATM withdrawals, cash deposits, and ATM transaction tracking.
   ---------------
*Conclusion: 
 -----------
These enhancements can make the Banking Management System more secure, reliable, and user-friendly. In the future, the system can be developed into a complete online banking application with advanced features.

Author:
--------
SQL Project — Banking Management System
