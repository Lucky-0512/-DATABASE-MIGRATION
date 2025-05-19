# Task 3: DATABASE MIGRATION
Company: CODTECH IT SOLUTIONS\
Name   : T V Sai Kushal\
Intern ID : CT04DL1133\
Domain : SQL / DBA\
Duration : 4 WEEKS\
Mentor : Neela Santhosh

## Task Description
Migrate data from a MySQL database (`source_db`) to a PostgreSQL database (`target_db`) while ensuring data integrity. Provide migration scripts and a summary of the process.

## Steps and Files

1. migration_mysql_to_postgresql.sh
   - A Bash script that:
     - Uses `mysqldump` to export the MySQL database schema and data.
     - Combines a cleaned‐up `schema_conversion.sql` (PostgreSQL DDL) with the `INSERT` statements from the MySQL dump.
     - Creates the target PostgreSQL database (if not already present).
     - Imports the combined SQL into PostgreSQL.
     - Verifies row counts for at least one example table (`employees`).\
       

2. schema_conversion.sql
   - Contains the PostgreSQL `CREATE TABLE` statements that replace MySQL tables.  
   - Example converts a MySQL `employees` table (with `AUTO_INCREMENT` and backticks) into a PostgreSQL‐compatible `SERIAL` and standard identifiers.

## Summary Report (Process Overview)

1. setting up MySQL and PostgreSQL.\
   ![Image](https://github.com/user-attachments/assets/56f3b0dc-860d-4e7b-8663-737fcc8f7d0b)

2. creating database and export db from mySQL.\
   ![Image](https://github.com/user-attachments/assets/238abada-fdaa-4294-acc4-c86f9a2498ca)

3. extracting INSERT queires from dump files\
   ![Image](https://github.com/user-attachments/assets/72e81053-92b5-42ce-b9d4-95ccf9d635b0)

4. import table into postGRE SQL.\
   ![Image](https://github.com/user-attachments/assets/a2be3f38-ee6d-4937-82af-cb2971c06069) 
   
