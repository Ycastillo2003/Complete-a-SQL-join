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

- We have now combined device_id column on the employees and machines tables, giving us a merged view of each machine assigned to an employee.
