SQL Bookstore Project

Description:
This project involves the design and implementation of a SQL database for a bookstore. The schema encompasses books, authors, and their relationships, and the repository includes various SQL scripts for creating tables, inserting data, stored procedures, and complex data retrieval queries.

Features:
Database Design: Comprehensive schema for books, authors, and their relationships.
Data Manipulation: Scripts for populating the database with sample data.
Stored Procedures: Implemented procedures like SellBook to simulate real-world operations.
Complex Queries: Examples of intricate SQL queries to fetch and analyze data.
Setup on MacOS

Requirements:
Docker - Ensure Docker is installed on your MacOS.
Azure Data Studio or any SQL client tool compatible with SQL Server.

Steps:
Running MSSQL Server using Docker:
bash
Copy code
docker pull mcr.microsoft.com/mssql/server
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=YourStrongPasswordHere' -p 1433:1433 --name sql_server -d mcr.microsoft.com/mssql/server
Connecting to the Database:
Open Azure Data Studio.
Click on New Connection.
Choose Microsoft SQL Server as the connection type.
For the server, input localhost.
Authentication type: SQL Login
Enter sa as the username and use the password you provided in the Docker command.
Click Connect.
Once connected, you can execute the SQL scripts from this repository in the order mentioned in the Usage section below.