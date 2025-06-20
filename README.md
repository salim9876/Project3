

# 🔐 Secure File Hider - Backend Application

This is a secure file management backend application built using **Java**, **JDBC**, and **MySQL**, allowing users to **hide/unhide files** securely. It features **OTP-based email verification** for user login/signup and manages file visibility based on authenticated sessions.

---

## 🚀 Features

- ✅ **User Registration & Login** with OTP verification via email
- 🔐 **Hide and Unhide Files** linked to a user's email
- 📬 OTP system implemented using **JavaMail API**
- 🗃️ **MySQL Database** for user and file information
- ⚙️ Console-based interactive UI
- 🧩 Modular design using DAO-Service-Model architecture
- 🔁 Continuous loop until user exits (Menu-driven app)

---

## 🛠️ Technologies Used

- **Java 17**
- **JDBC (without JPA)**
- **MySQL**
- **JavaMail API** (SMTP for Gmail)
- **Maven** (for dependency management)

-
## 🗂️ Project Structure
src/
├── dao/
│ └── UserDAO.java, DataDAO.java
├── model/
│ └── User.java, Data.java
├── service/
│ └── SendOTPService.java, GenerateOTP.java, UserService.java
├── views/
│ └── Welcome.java, UserView.java
└── Main.java

pgsql
Copy
Edit


---

## 🧾 Database Schema

```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100) UNIQUE
);

CREATE TABLE files (
    id INT AUTO_INCREMENT PRIMARY KEY,
    file_name VARCHAR(255),
    path TEXT,
    email VARCHAR(100)
);



---

How to Run
🔧 Prerequisites
Java 17

MySQL installed and running

Gmail credentials (for sending OTP)

Maven
 Setup Steps
Clone or download the repository

Update your Gmail credentials in SendOTPService.java:
Configure your MySQL connection in MyConnection.java

Create the required tables in MySQL using the schema above

Run the application:

bash
Copy
Edit
📸 Sample Flow
Welcome to the app
1. Login
2. Signup
0. Exit

> Enter Email
> OTP sent to email
> File Hide/Unhide Menu appears after login
