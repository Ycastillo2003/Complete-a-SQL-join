![image](https://github.com/user-attachments/assets/55c66eb5-ce90-4351-8fe4-4bdf843d3556)


# SQL: Complete a SQL join.
This project involved writing and executing SQL queries using various types of joins to combine data across multiple related tables in a database. The objective was to retrieve meaningful, connected information by using INNER JOIN, LEFT JOIN, and RIGHT JOIN clauses based on shared key fields.

# Environments and Technologies Used.
- Google Cloud Virtual Machines.
- SQL (Structured Query Language).

# Operating Systems Used </h2>
- Linux.

# Actions and observations.
- First, we must identify which employees are using which machines. The data is located in the machines and employees tables.

![image](https://github.com/user-attachments/assets/114ad5ee-1f80-4ab9-a1e0-80efed1e86e7)![image](https://github.com/user-attachments/assets/e95c08d2-176f-48a3-97a8-0980fec16647)

- We must use a SQL INNER JOIN to return the records we need based on a connecting column. In this scenario, both tables include the device_id column, which we’ll use to perform the join.

![image](https://github.com/user-attachments/assets/c9fd1caf-ed73-412e-9a18-8495c0d4bb60) ![image](https://github.com/user-attachments/assets/b972d8dc-10b5-4a33-9f7a-7c0817b14df8)

- We have now combined the device_id column on the employees and machines tables, giving us a merged view of each machine assigned to an employee.

We must now return the information on all machines and the employees who have machines. Next, we'll do the reverse—retrieving the information of all employees and any machines that are assigned to them.

To achieve this, we’ll complete a LEFT JOIN and a RIGHT JOIN on the employees and machines tables. These joins will allow us to include all records from one of the tables, regardless of whether a match exists in the other. We will link the tables using the common column: device_id.

![image](https://github.com/user-attachments/assets/b9116721-d786-460a-b40d-0d4867cffa61) ![image](https://github.com/user-attachments/assets/22e7e770-92c6-4c09-9041-7779e55af836)

- In this case, all records from the machines table are included, regardless of whether they are assigned to an employee or not.

![image](https://github.com/user-attachments/assets/544791a9-33d7-46db-b9a8-2baf7b88b56b)![image](https://github.com/user-attachments/assets/1165693d-64c6-42e1-b2b5-2074a3238d4d)

- This RIGHT JOIN combines the machines and employees tables using the device_id column. It returns all rows from the employees table, along with matching machine details when available. If an employee does not have a machine assigned, the machine's columns will show NULL.


     WE must investigate a security incident, we must retrieve the information on all employees who have made login attempts. To achieve this, we’ll perform an INNER JOIN on the employees and log_in_attempts tables, linking them on the common username column.

![image](https://github.com/user-attachments/assets/8df40b14-2b0a-47ed-a710-3af39cda1d82)![image](https://github.com/user-attachments/assets/ef0956a5-e11d-4924-8297-d9c502dc72d7)

This query links the employees table (which contains employee details) with the log_in_attempts table (which logs login activity). By joining them on the username, we get a unified view that shows which employee attempted a login and the details of that attempt.


   Thanks for making it to the end of this lab.
