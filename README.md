# SQL Bookstore Project

## Description
The goal of this SQL Bookstore Project create a robust MS SQL database system tailored for a bookstore environment. This repository contains the necessary SQL scripts for constructing a comprehensive schema that involves entities such as books, authors, and their interrelations. The aim is to provide a suite of scripts for establishing table structures, populating them with sample data, and crafting stored procedures and complex queries that mimic real-world data retrieval and manipulation.

## Features

- **Database Design**: Detailed schema design capturing books, authors, and the relationships between them.
- **Data Manipulation**: Provision of scripts for adding sample data to the database to simulate a real bookstore.
- **Stored Procedures**: Includes procedures like `SellBook` to carry out typical bookstore transactions.
- **Complex Queries**: Offers a collection of sophisticated SQL queries for data retrieval and analytics.

## Setup on MacOS

### Requirements

- **Docker**: Make sure Docker is installed and running on your MacOS system.
- **Azure Data Studio** or any other SQL client tool that supports SQL Server.

### Installation Steps

#### Running MSSQL Server using Docker:

```bash
docker pull mcr.microsoft.com/mssql/server
docker run -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=YourStrongPasswordHere' -p 1433:1433 --name sql_server -d mcr.microsoft.com/mssql/server

Connecting to the Database:

Open Azure Data Studio.
Click on New Connection.
Select Microsoft SQL Server as the connection type.
For the server, input localhost.
Authentication type: Select SQL Login.
Enter sa as the username.
Use the password you set (YourStrongPasswordHere) in the Docker run command.
Click Connect.
After connecting, you're all set to execute the SQL scripts provided in this repository.

