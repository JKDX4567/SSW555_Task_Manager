# SSW555_Task_Manager
Group Project for SSW555

## Database Installation
1. Run the command ```psql -U postgres```
2. Create the postgres database using ```CREATE DATABASE task_manager;```
3. Switch to the database using ```\c task_manager```
4. Create the accounts table using 
```
CREATE TABLE accounts ( 
    id SERIAL PRIMARY KEY,
    email TEXT UNIQUE NOT NULL,
    password TEXT NOT NULL
);
```
