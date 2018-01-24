#Types of Normalization forms

Normalization of DB tables is something like 'Ensuring Single Responsibility principle and Ensuring cohesion' with classes.

There are many types of Normalization forms.
We want to understand 3NF or **Third Normal Form**

##First Normal Form
Let us look at the Employee Table:
-Employee
--Employee ID
--First Name
--Second Name
--CellPhone1
--CellPhone2
--CellPhone3

Now, there is a problem here from First Normal Form point of view.
We want to ensure that **There should be NO REPEATING Columns for a table to be in First Normal Form **

Here is how the table would look in First Normal Form:
-Employee
--Employee ID
--First Name
--Second Name
--CellPhones

##Second Normal Form
Let us look at the Employee Table below:
--Employee
--Employee ID(Primary Key)
--First Name
--Second Name
--CellPhone
--Sales Office
--Office Number

Now if we ask a question:
**Does Every column serve to describe what the Primary key identifies?If no, then move that column to another table**
If the EmployeeID identifies the 'Employee', then the Sales Office column does not help to identify an Employee
We should move the Sales Office and Office Number out of this table.

Another Example:
-Customer
--CustomerID (PK)
--Employee ID(FK)
--Customer Name
--Customer City
--Customer Postal Code

Now, the question here is : Does the "Employee ID" Primary key help to identify Customer? Do the Customer Name, Customer City, Customer Postal Code depend upon the Employee ID to correctly identify the Customer?

The problem here is the Employee ID Foriegn Key.
Question: if there is ONLY one key in the primary key, does 2NF apply?
##Third Normal Form
Are there two or more columns which represent the same data?
For example City Namd and PIN Code are two things which represent the same information
Another example is Age and Date of birth are two columns which show the same information in two ways.
This is an area where data inconsistency can creep in.


