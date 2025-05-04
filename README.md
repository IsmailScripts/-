Library Management System

Overview

The Library Management System (LMS) is a web-based application designed to streamline the management of library operations, reducing the complexity and manual effort involved in traditional library systems. This project aims to provide an efficient and user-friendly platform for librarians, students, and teachers to manage books, track borrowing activities, and facilitate book requests. Key features include admin and student login systems, book issuance tracking, and a request mechanism for recommending new books.

Developed as a group project by:
Muhammad Ismail Awan (22K-4225)

Features

Admin Login: Allows librarians to manage books, users, book requests, and dues, and view reports.
Student Login: Enables students to view issued books, check issue/return dates, calculate dues, and request new books.
Book Management: Add, remove, and update book details, including availability and pricing.
Search and Request: Users can search for books by availability and submit requests for new titles.
Reports: Generate reports for book requests, issued books, and user activity.
User Dashboard: Displays personal information, recent check-ins/checkouts, and borrowing status.
Error Handling: Manages expected and unexpected errors to prevent data loss and ensure system reliability.
Security: Restricts database modifications to authorized admin users and supports high user/book volumes.

System Environment

Front-End
HTML
CSS
Bootstrap

Back-End
PHP
MySQL

Tools & Technologies
Xamp Server
MySQL Queries
Browser: Google Chrome

Database Structure
The LMS uses a MySQL database named BMS with the following tables:
Admin (id as primary key): Stores admin details.
Book (id as primary key): Stores book details (name, author, price, availability, etc.).
IssueBook (id as primary key): Tracks book issuance details (user, issue date, etc.).
RequestBook (id as primary key): Manages book request data.
UserData (id as primary key): Stores user details (students and teachers).

Functional Requirements
Store and manage admin and user information (login details, issued books, etc.).
Maintain book and user data in a MySQL database.
Support book/journal searches by availability.
Generate reports for book requests to aid librarian decision-making.
Allow users to view personal details, borrowing status, and recent transactions.
Provide modules for searching and requesting books.
Enable librarians to manage books, users, dues, and recommendations.

Non-Functional Requirements
Usability: Simple, interactive, and intuitive user interface with clear login prompts.
Error Handling: Robust mechanisms to prevent data loss and minimize downtime.
Security: Restrict database modifications to authorized admins and ensure scalability.

Performance: Handle large numbers of books and users without faults.

Installation
Prerequisites:
Install Xampp Server (includes Apache, PHP, and MySQL).
Ensure Google Chrome is installed for testing.

Setup:
Clone the repository: git clone <repository-url>.
Place the project folder in the www directory of Wamp Server (e.g., C:\wamp64\www\lms).
Start Xampp Server and ensure Apache and MySQL services are running.

Database Configuration:
Open phpMyAdmin (http://localhost/phpmyadmin).

Create a database named BMS.
Import the SQL file (bms.sql) from the project directory to set up tables and initial data.
Update database connection settings in the PHP configuration file (e.g., config.php) with your MySQL credentials:
$host = 'localhost';
$user = 'root';
$password = '';
$database = 'BMS';

Run the Application:
Open Google Chrome and navigate to http://localhost/lms.
Log in as an admin or student to explore the system.

Usage
Admin Access:
Log in with admin credentials to add/remove books, manage users, process dues, and view book requests.
Use the "Book Report" and "Issued Book Record" pages to monitor library activity.

Student Access:
Log in to view issued books, check return dates, calculate dues, and submit book requests via the "Request Book" feature.
Use the student dashboard to track borrowing history and personal details.



