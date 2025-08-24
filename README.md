# 🎓 Student Result Management System v2.0

Student Result Management System v2.0 – A PHP &amp; MySQL-based web application for managing student records, results, and performance reports with an admin-friendly dashboard.

<img width="1914" height="862" alt="SRMS-Home" src="https://github.com/user-attachments/assets/2a1974dc-b1c2-444d-a564-69de44cc5b6e" />

📌 Overview

The Student Result Management System (SRMS) is a web-based application built using PHP & MySQL that helps schools, colleges, and universities efficiently manage student records and results.

It provides an Admin Panel for managing classes, students, and results, and a Student Panel where students can check their results online securely.


✨ Features

<img width="1920" height="864" alt="SRMS-admin page" src="https://github.com/user-attachments/assets/4e64b8a3-aa43-4771-b00e-baf86b7d96c0" />

🔑 Admin Panel

* Manage classes & subjects

* Add, update & delete student records

* Enter and publish student results

* Generate performance reports

<img width="1920" height="860" alt="SRMS-login" src="https://github.com/user-attachments/assets/97e7af55-abd9-4f3c-a99d-0a5d801d55d2" />

🎓 Student Panel

* Search results by Roll Number

* View marks, grades, and overall performance

* Secure & role-based access


⚡ General

*  User authentication & session management

* Responsive UI for easy access

* MySQL database for storing records securely

🛠️ Tech Stack

* Frontend

* HTML5, CSS3, Bootstrap

* JavaScript

* Backend

* PHP (Core PHP v7+ / v8 supported)

* Database

* MySQL (via phpMyAdmin in XAMPP/WAMP/MAMP)

# Tools

* XAMPP / WAMP (for local development)

* VS Code (as IDE)

* phpMyAdmin (for database management)


📂 Project Structure

Student-Result-Management-System/

│── admin/                # Admin Panel

│── student/              # Student Panel

│── includes/             # Database connection & helper files

│── database/             # SQL file for database import

│── index.php             # Homepage

│── login.php             # Admin login

│── README.md             # Project documentation


🚀 Installation & Setup

1. Install XAMPP / WAMP

* Download & install XAMPP

* Start Apache & MySQL from Control Panel.

2. Setup Project

* Copy project folder to htdocs directory:
  
* C:\xampp\htdocs\Student-Result-Management-System

3. Configure Database

* Open http://localhost/phpmyadmin

* Create a database named srms.

* Import the srms.sql file from the database/ folder.

4. Configure Database Connection

* Edit includes/config.php (or similar) and update:

<?php
$host = "localhost";
$user = "root";      // default MySQL user
$pass = "";          // default password is empty
$db   = "srms";      // your database name

$conn = mysqli_connect($host, $user, $pass, $db);

if (!$conn) {
    die("Database Connection Failed: " . mysqli_connect_error());
}
?>

5. Run the Project

* Open browser and go to:

* http://localhost/Student-Result-Management-System/

🔐 Default Credentials

* Admin Login

* Username: admin

* Password: admin123

* Student Login

* Roll number-based access (as per database records)

📊 Future Enhancements

📌 Role-based user management (Teachers, Parents)

📌 Export results to PDF/Excel

📌 Email/SMS notifications to students

📌 Enhanced security (password hashing, captcha, etc.)

📜 License

This project is licensed under the MIT License – free to use, modify, and distribute.
