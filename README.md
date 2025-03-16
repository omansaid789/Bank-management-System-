# Bank-management-System-
ES-221 Project 
This is a basic implementation of a Banking System in C++ in which Data Structures are used.
**Introduction**
The Banking Management System is a C++ program designed to simulate basic banking operations such as adding customers, managing transactions (deposits and withdrawals), and displaying customer details. The system leverages various data structures to efficiently store, retrieve, and manage customer information and transactions. This project demonstrates the practical application of data structures like linked lists, hash tables, binary search trees (BST), and queues in a real-world scenario.
 **Objectives**
The primary objectives of this project are:
•	To implement a basic banking system that allows customers to create accounts, deposit funds, withdraw funds, and view their transaction history.
•	To demonstrate the use of data structures for efficient data management and retrieval.
•	To provide a user-friendly interface for interacting with the banking system.
**Features**
•	Add Customer: Allows the bank to add a new customer with details such as name, PIN, address, contact number, and email.
•	Display Customer Details: Displays customer information and transaction history after verifying the account number and PIN.
•	Deposit Funds: Allows customers to deposit money into their account.
•	Withdraw Funds: Allows customers to withdraw money from their account, provided they have sufficient balance.
•	Transaction History: Maintains a record of all transactions (deposits and withdrawals) for each customer.
**Implementation Details**
Customer Management
Adding a Customer:
•	The add_customer() method in the Bank class takes user input to create a new customer. 
•	The customer is added to the linked list, and the account number is mapped to the customer's iterator in the hash table.
•	The customer is also inserted into the BST for efficient searching.

**Displaying Customer Details:**
•	The display_user(int accnum, int PIN) method searches for the customer using the account number in the BST.
•	If the PIN matches, the customer's details and transaction history are displayed.
Transaction Operations
**Depositing Funds:**
•	The deposit(int accnum, int PIN, double amount) method searches for the customer using the account number in the BST.
•	If the PIN matches, the specified amount is added to the customer's balance, and the transaction is recorded.
Withdrawing Funds:
•	The withdraw(int accnum, int PIN, double amount) method
•	searches for the customer using the account number in the BST.
•	If the PIN matches and the customer has sufficient balance, the specified amount is deducted from the balance, and the transaction is recorded.
**Main Function: **
Displays a menu for the user with options to add a customer, display customer details, deposit, withdraw, or exit. The user interacts with the system by choosing options based on their needs. The program uses the Bank class methods to perform the specified operations. Conclusion: The program provides a basic banking management system with customer information stored in a linked list, efficient retrieval using a hash table, and fast account number searches using a binary search tree. It also supports transaction history and basic deposit/withdraw functionalities.
**Conclusion**
The Banking Management System is a functional and efficient program that demonstrates the use of various data structures to manage customer data and transactions. While it has some limitations, it provides a solid foundation for further development and enhancement. With additional features and improvements, it can be transformed into a fully-fledged banking application.
