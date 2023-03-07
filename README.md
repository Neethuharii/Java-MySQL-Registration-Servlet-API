
# Login Page Servlet API

This is a simple servlet API for a login page. 
This repository contains Java code for a basic student registration system.
The code provides a servlet for a web application that allows users to register student 
information such as name, age, and mark into a MySQL database. The system uses JDBC to connect to
the database and insert the information. The repository includes instructions for setting up and 
using the system

## Description

This servlet API takes user input for name, age and marks and saves it to a MySQL database using JDBC. It connects to a database with the URL `jdbc:mysql://localhost:3306/bmc`, where `bmc` is the name of the database. The username and password for the database are hardcoded as `root` and `root`.

## Usage

To use this API, you need to send a GET request to the URL `/reg` with the following parameters:
- `stname`: The name of the student.
- `stage`: The age of the student.
- `stmark`: The marks of the student.

The API then saves this data to the MySQL database.

## Dependencies

This servlet API depends on the following:
- Java Development Kit (JDK) version 8 or higher
- MySQL database
- MySQL Connector/J driver for JDBC

## How to run

1. Clone this repository to your local machine.
2. Open the project in your Java IDE.
3. Make sure you have the dependencies listed above installed and available in your project.
4. Run the `RegistrationServlet` class. 
5. Open your web browser and go to `http://localhost:8080/reg?stname=<name>&stage=<age>&stmark=<mark>`, where `<name>`, `<age>`, and `<mark>` are the values you want to save to the database.
6. The API will save the data to the MySQL database and display the message "saved successfully" in the browser.

Note: Make sure to change the username and password to match your own MySQL database configuration.
