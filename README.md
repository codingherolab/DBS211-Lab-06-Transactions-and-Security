# DBS211-Lab-06-Transactions-and-Security

Download Here: [DBS211 Lab 06 – Transactions and Security](https://codingherolab.com/product/dbs211-lab-06-transactions-and-security/)

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

Objective:
Submission:
Your submission will be a single text-based SQL file with the solutions provided.

Your submission needs to contain a comment header block and be commented and include the question number and the solutions. Make sure every SQL statement terminates with a semicolon.

You will use following data to complete the given tasks:

employeeNumber	lastname	firstname	extension	email	OfficeCode	reportsTo	jobTitle
100	Patel	Ralph	22333	rpatel@mail.com	1	NULL	Sales Rep
101	Denis	Betty	33444	bdenis@mail.com	4	NULL	Sales Rep
102	Biri	Ben	44555	bbirir@mail.com	2	NULL	Sales Rep
103	Newman	Chad	66777	cnewman@mail.com	3	NULL	Sales Rep
104	Ropeburn	Audrey	77888	aropebur@mail.com	1	NULL	Sales Rep
SET TRANSACTION READ WRITE starts a new transaction.
COMMIT commits the current transaction, making its changes permanent.
SAVEPOINT <name> sets a pointer to a location that can be rolled back to.
ROLLBACK rolls back the current transaction, canceling its changes.
SET autocommit disables or enables the default autocommit mode for the current session.
Tasks:

It is very important that these tasks be performed in the order presented here for maximum learning.

PART A – Transactions
List the 4 ways that we know that a transaction can be started
Transaction, Commit, Save Point and Rollback.

Using SQL, create an empty table, that is the same as the employees table, and name it newEmployees.
Execute the following commands.
SET AUTCOMMIT OFF;
SET TRANSACTION READ WRITE;

 

Write an INSERT statement to populate the newEmployees table with the rows of the sample data. Insert the NULL value for the reportsTo column. (Write a single INSERT statement to insert all the rows)
 

Create a query that shows all the inserted rows from the newEmployees table. How many rows are selected?
 

Execute the rollback command. Display all rows and columns from the newEmployees table. How many rows are selected?
 

Repeat Task 4. Make the insertion permanent to the table newEmployees. Display all rows and columns from the newEmployee table. How many rows are selected?
 

Write an update statement to update the value of column jobTitle to ‘unknown’ for all the employees in the newEmployees table.
 

Make your changes permanent.
 

Execute the rollback command.
Display all employees from the newEmployees table whose job title is ‘unknown’. How many rows are still updated?
Was the rollback command effective?
What was the difference between the result of the rollback execution from Task 6 and the result of the rollback execution of this task?
Begin a new transaction and then create a statement to delete to employees from the newEmployees table
Create a VIEW, called vwNewEmps, that queries all the records in the newEmployees table sorted by last name and then by first name.
Perform a rollback to undo the deletion of the employees
How many employees are now in the newEmployees table?
Was the rollback effective and why?
Begin a new transaction and rerun the data insertion from Task 4 (copy the code down to Task 14 and run it)
Set a Savepoint, called insertion, after inserting the data
Rerun the update statement from Task 8 and run a query to view the data (copy the code down and run it again)
Rollback the transaction to the Savepoint created in task 15 above and run a query to view the data.
What does the data look like (i.e. describe what happened?
Use the basic for of the rollback statement and again view the data. Describe what the results look like and what happened.
Part B – Permissions
Write a statement that denies all access to the newemployees table for all public users
Write a statement that allows a classmate (use their database login) read only access to the newemployees table.
Write a statement that allows the same classmate to modify (insert, update and delete) the data of the newemployees table.
Write a statement the denies all access to the newemployees table for the same classmate.
Part C – Clean up
Write statements to permanently remove the view and table created for this lab
 

 

 
