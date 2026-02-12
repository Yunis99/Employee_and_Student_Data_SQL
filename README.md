# SQL Database Design and Data Manipulation Project

## Disclaimer

This project was developed for educational purposes to demonstrate SQL database design, data manipulation, and date-based scripting techniques.

---

## Project Overview

This project involves the creation and manipulation of relational database tables using SQL. The focus is on table creation with constraints, conditional data updates, deletions, and date-based calculations. The project simulates real-world data management tasks using Employees and Students datasets.

---

## Database Design

### Tables Created

1. **STUDENTS**
   - s_id (Primary Key)
   - first_name (*Not Null)
   - last_name (*Not Null)
   - email
   - phone_number
   - Other attributes as required

2. **ACTIVITIES**
   - activity_id (Primary Key)
   - activity_name (*Not Null)

3. **SCHEDULE**
   - schedule_id (Primary Key)
   - s_id (Foreign Key referencing STUDENTS)
   - activity_id (Foreign Key referencing ACTIVITIES)
   - scheduled_date

4. **PROGRAMMERS**
   - Derived from EMPLOYEES table
   - Contains records where job_id contains 'PROG'

5. **PARTICIPANTS**
   - first_name
   - last_name
   - salary (>10000)

---

## Data Manipulation Operations

1. **Data Migration**
   - Inserted records into STUDENTS table from EMPLOYEES table.

2. **Conditional Updates**
   - Masked phone numbers as '***' for students where s_id > 200.
   - Updated first_name and last_name values to uppercase.
   - Updated email to 'DSA' for records where s_id > 150.

3. **Conditional Deletions**
   - Deleted records from STUDENTS where s_id is between 150 and 160.

4. **Table Maintenance**
   - Inserted sample data into SCHEDULE table.
   - Applied TRUNCATE to remove all records.
   - Dropped the SCHEDULE table entirely.

---

## Date-Based SQL Scripting

For any given date, the following calculations were performed:

- First and last days of the next year
- First and last days of the next month
- First and last days of the previous month

This demonstrates proficiency in date arithmetic and built-in date functions.

---

## Skills Demonstrated

- Relational database design and normalization
- Primary and foreign key constraints
- Data migration between tables
- Conditional updates and deletions
- Table truncation and dropping
- Date calculations and scripting
- Conditional table creation based on data
- Advanced SQL DDL and DML operations

---

## Tools Used

- SQL (Oracle, MySQL, or PostgreSQL)
- Database management and querying
- SQL functions for date arithmetic

---

## Key Learning Outcomes

- Understanding relational database management principles
- Managing data integrity with constraints
- Performing complex data manipulation tasks
- Writing date-aware SQL scripts
- Transforming business requirements into database operations

---

## Future Improvements

- Implement stored procedures for automated tasks
- Create triggers for data validation
- Optimize queries for performance
- Integrate reporting views for student and activity tracking
