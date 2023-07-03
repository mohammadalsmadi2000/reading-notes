# Reading Notes: Permissions & Postgresql

## Why does this topic matter?
Understanding permissions in Django Rest Framework (DRF) and working with SQL SELECT statements are crucial skills for building secure APIs and manipulating data in databases. These topics directly relate to the module I am studying as they provide the foundation for handling user access control and retrieving data from a database.

## DRF Permissions
### Key components and purpose of DRF permissions:
DRF permissions provide a way to control access to views in an API by determining whether a user should be allowed to perform a certain action.
Key components include:
- Permissions classes: These classes define the access rules and are applied to views.
- Permission checks: These checks are performed when a user tries to access an API endpoint and determine if the user has the necessary permissions.
### Purpose:
DRF permissions help in securing an API by ensuring that only authorized users can perform certain actions, such as creating, updating, or deleting data.
They provide a fine-grained control over access to views based on user roles, authentication status, object ownership, or custom business logic.

## SQL SELECT Statement
### Purpose of the SELECT statement:
The SELECT statement in SQL is used to retrieve data from one or more tables in a database.
It allows us to specify the columns we want to retrieve and apply filters to narrow down the results.
The SELECT statement is fundamental for querying and manipulating data in a database.
### Retrieving all columns from a table called 'employees':
To retrieve all columns from the 'employees' table, the following SQL query can be used:
```sql
SELECT * FROM employees;
```
The asterisk (*) symbol represents all columns in the table, and the query will return all rows and columns from the 'employees' table.


## Things I want to know more about
* How can custom permissions be implemented in DRF?
* Are there any performance considerations when using DRF Generic Views?
* How can I optimize SQL SELECT queries for large datasets?
* Can I use PostgreSQL-specific features in conjunction with DRF?
* What are some best practices for securing APIs with DRF permissions?

