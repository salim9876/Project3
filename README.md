# Project3
File Hider
# 🔐 File Hider

A secure Java-based application that allows users to **hide/unhide personal files or folders** using a clean UI with OTP-based login verification. It ensures privacy and adds an extra layer of protection for sensitive data.

![Screenshot](proj_3.jpg)

---

## 🚀 Features

- 🔑 **OTP-based User Login**  
- 🔐 **Hide and Unhide Files/Folders**  
- 💽 **Secure File Encryption Handling**  
- 📂 **Drag-and-Drop File Support**  
- 📧 **OTP sent via Email using JavaMail API**  
- 🖥️ **Java Swing GUI for Easy Use**

---

## 🧰 Tech Stack

- Java 8+
- Maven
- MySQL
- JDBC
- Java Swing
- JavaMail API (OTP Emailing)
- Spring Boot
---

## 📁 Project Structure
File Hider/
├── pom.xml
├── src/
│ ├── dao/
│ ├── model/
│ ├── service/
│ ├── views/
│ └── Main.java

---

## ⚙️ Setup Instructions

### 🛑 Prerequisites

- Java 8+ installed
- Maven installed
- MySQL server running
- Gmail account for OTP emailing

### 🧪 Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/FileHider.git
cd FileHider

# Compile the project
mvn clean install

# Run the app
mvn exec:java -Dexec.mainClass="Main"
Database Setup
Create MySQL database file_hider_db

Update your DB credentials in MyConnection.java

Run the SQL table script (if provided) or let the app handle it

🎯 Usage
Run the app

Enter email → Receive OTP → Login

Drag and drop files/folders into the interface

Click on Hide File or Unhide File

