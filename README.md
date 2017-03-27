# Student-Database-System-with-Btrees-and-List
I have simulated some functionality of a database system. It is assumed that a number of users want to access a student database and perform the following functions:

1. Create a student record (C)
2. Review a student record (R)
3. Update a student record (U) (other than roll number)
4. Delete a student record (D)

In addition, a user may want to view students’ data from a given roll number to another roll number in ascending or descending order.
User may also want to view all students’ records.

The student record contains the following information:
a) Roll Number
b) Name
c) List of courses taken and grades earned

The student data is stored in a sorted doubly linked-list.
In order to speed-up all the operations, a B tree based index is created. The student Roll No. will serve as the key. Each node in the tree will store the pairs (key and a pointer to the student data stored in a doubly linked-list).

At any point in time, the data may be stored in a file or retrieved from a file. When the data is retrieved, a new B tree and the corresponding doubly linked-list is constructed.
At each execution of the program the user would be asked to either load the data from a file or give the order of the B tree (value of t) to create a new one to perform the database operations.
