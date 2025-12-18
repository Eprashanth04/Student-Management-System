# Student Management System (Java + JDBC + MySQL)

A **console-based Student Management System** developed using **Core Java, JDBC, and MySQL**. This project demonstrates fundamental backend development concepts such as database connectivity, CRUD operations, and clean menu-driven program design.

---

## 📌 Features

* Add new student records
* View all students
* Update existing student details
* Delete student records
* Search student by ID
* Menu-driven console interface

---

## 🛠 Tech Stack

* **Language:** Java (Core Java)
* **Database:** MySQL
* **Database Connectivity:** JDBC
* **IDE:** VS Code / Eclipse / IntelliJ
* **Architecture:** Console-based, procedural flow

---

## 🗂 Project Structure

```
StudentManagementSystem/
│
├── StudentManagementSystem.java
├── README.md
└── database.sql
```

---

## ⚙️ Database Setup (MySQL)

Create the database and table using the following SQL commands.

```sql
-- Create Database
CREATE DATABASE studentdb;

-- Use Database
USE studentdb;

-- Create Students Table
CREATE TABLE students (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    age INT,
    course VARCHAR(50)
);
```

Save this as **`database.sql`** and execute it in MySQL Workbench or command line.

---

## 🔌 JDBC Configuration

Update the database credentials in the Java file:

```java
static final String URL = "jdbc:mysql://localhost:3306/studentdb";
static final String USER = "root";
static final String PASSWORD = "your_password";
```

Ensure **MySQL Connector/J** is added to your project libraries.

---

## ▶️ How to Run the Project

1. Clone the repository

   ```bash
   git clone https://github.com/your-username/student-management-system-jdbc.git
   ```
2. Import the project into your IDE
3. Add MySQL Connector JAR to the build path
4. Run `StudentManagementSystem.java`
5. Use the menu options to perform operations

