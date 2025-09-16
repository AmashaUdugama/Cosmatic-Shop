  Cosmetic Shop Management System
A Java desktop application for managing cosmetic shop operations with MySQL database integration.
✨ Features

🛍️ Product inventory management
👥 Customer registration & management
🧾 Sales & billing system
📊 Stock tracking & reports
🔐 Admin authentication
💾 MySQL database integration

📋 Prerequisites

☕ Java JDK 8+
🗄️ MySQL Server
📚 MySQL Connector
🔧 IDE (NetBeans)

🚀 Installation

Clone the repository

bashgit clone https://github.com/AmashaUdugama/Cosmatic-Shop.git


Setup MySQL Database

sqlCREATE DATABASE accounts;
USE accounts;

-- Run the provided SQL schema file
SOURCE database/schema.sql;

Configure Database Connection
Update connectionProvider.java with your MySQL credentials:

javaString url = "jdbc:mysql://localhost:3306/accounts";
String user = "root";
String password = "your_mysql_password";

Add MySQL Driver to Classpath


Download MySQL Connector/J JAR file
Add to your IDE's project libraries
Or place in lib/ folder


Compile and Run

bash# Compile
javac -cp "lib/mysql-connector-java.jar" src/*.java

# Run
java -cp "src:lib/mysql-connector-java.jar" Main
🛠️ Tech Stack
Language: ☕ Java SE
Database: 🗄️ MySQL
GUI Framework: 🖼️ Java Swing
Database Connectivity: 🔌 JDBC
Build Tool: 🔨 Maven/Gradle (optional)
📁 Project Structure
Cosmatic-Shop/
├── src/
│   ├── connectionProvider.java    # Database connection utility
│   ├── Main.java                  # Application entry point
│   ├── LoginForm.java             # User authentication
│   ├── ProductManager.java        # Product CRUD operations
│   ├── CustomerManager.java       # Customer management
│   ├── SalesManager.java          # Sales & billing
│   └── DatabaseHelper.java        # Database utilities
├── lib/
│   └── mysql-connector-java.jar   # MySQL JDBC driver
├── database/
│   └── schema.sql                 # Database schema
└── README.md
