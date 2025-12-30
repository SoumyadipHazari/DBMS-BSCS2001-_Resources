# Week 1

## 🧑‍💻Lecture 1.1 (Why DBMS?/1)

### **Database Management System (DBMS)**

Database Management System is a **Software system** which helps us to store, organize, manage and retrieve from a database

DBMS helps us in
- 
- Storing data in a structured way (in a table using row and columns)
- Fast searching
- Data remains consistent
- No unnecessary duplication
- Updating the data in a very easy way
- Make the data accessible to the particular users
- Access data at the same time with multiple users without conflict
- Backup or recovery of the data if any failures happens

🥸 Example
- 
Below is a small database where different columns consists the data about students like name, roll no. and marks
| Roll No | Name   | Marks |
| ------- | ------ | ----- |
| 1       | Rahul  | 85    |
| 2       | Anjali | 90    |

here we can easily add students with details and it will also helps us to search for a particular entry (rows containing details of different students)

Drawbacks of file system to store data 
-
- Data **redundancy** (it means the same data is stored multiple times in different places.) and **inconsistency** (means different copies of the same data do not match.)
- Getting problems during accessing data
- Data **isolation** (it is a situation where data is scattered across multiple, separate files or systems, and one application cannot easily access or combine data managed by another application.)
- May happen failure in **Atomicity** (a database operation is treated as a single, indivisible unit: either all changes happen, or
none of them happen at all) (update happens half) like 

    - Suppose ₹1000 is transferred from Account A to Account B. that means
    
      1. Deduct ₹1000 from Account A
      2. Add ₹1000 to Account B

    - What can go wrong without atomicity?

            If the system crashes after step 1 but before step 2:

            Account A loses money

            Account B does not receive it

