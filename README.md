# SSW555_Task_Manager
Group Project for SSW555

## Database Installation and Setup
1. Run the command ```psql -U postgres``` in your terminal 
2. Create the postgres database using ```CREATE DATABASE task_manager;```
3. Switch to the database using ```\c task_manager```
4. Create the `accounts` table using 
```
CREATE TABLE accounts ( 
    id SERIAL PRIMARY KEY,
    name TEXT NOT NULL,
    email TEXT UNIQUE NOT NULL,
    password TEXT NOT NULL
);
```
5. Create the `tasks` table using
   ```
   CREATE TABLE tasks ( 
    id SERIAL PRIMARY KEY,
    status,
    category,
    due_date,
    title TEXT NOT NULL,
    description TEXT
    );
    ```
6. Type `\q` to exit Postgres
