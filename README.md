# 💄 Cosmetic Shop Management System

A Java desktop application for managing cosmetic shop operations with MySQL database integration.

## ✨ Features

- 🛍️ Product inventory management
- 👥 Customer registration & management
- 🧾 Sales & billing system
- 📊 Stock tracking & reports
- 🔐 Admin authentication
- 💾 MySQL database integration

## 📋 Prerequisites

- ☕ [Java JDK 8+](https://www.oracle.com/java/technologies/downloads/)
- 🗄️ [MySQL Server](https://dev.mysql.com/downloads/mysql/)
- 🔧 IDE ( NetBeans)

## 🚀 Installation

1. **Clone the repository**
```bash
git clone https://github.com/AmashaUdugama/Cosmatic-Shop.git
cd Cosmatic-Shop
```

2. **Setup MySQL Database**
```sql
CREATE DATABASE accounts;
USE accounts;

-- Run the provided SQL schema file
SOURCE database/schema.sql;
```

3. **Configure Database Connection**
Update `connectionProvider.java` with your MySQL credentials:
```java
String url = "jdbc:mysql://localhost:3306/accounts";
String user = "root";
String password = "your_mysql_password";
```

4. **Add MySQL Driver to Classpath**
- Download MySQL Connector/J JAR file
- Add to your IDE's project libraries
- Or place in `lib/` folder

5. **Compile and Run**
```bash
# Compile
javac -cp "lib/mysql-connector-java.jar" src/*.java

# Run
java -cp "src:lib/mysql-connector-java.jar" Main
```

## 🛠️ Tech Stack

**Language:** ☕ Java SE  
**Database:** 🗄️ MySQL  
**GUI Framework:** 🖼️ Java Swing  


## 📁 Project Structure

```
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
```

## 🚦 How to Run

1. **Start MySQL Server**
```bash
# Windows
net start mysql

# macOS
brew services start mysql

# Linux
sudo systemctl start mysql
```

2. **Open in IDE**
- Import project into your Java IDE
- Add MySQL Connector JAR to build path
- Configure database connection settings

3. **Run Application**
- Execute `Main.java`
- Login with admin credentials
- Start managing your cosmetic shop!

## 📱 Application Modules

### 🔐 Authentication
- Admin login system
- Session management
- User role validation

### 🛍️ Product Management
- Add/Edit/Delete products
- Category management
- Stock level tracking
- Price management

### 👥 Customer Management
- Customer registration
- Profile management
- Purchase history tracking

### 🧾 Sales & Billing
- Point of sale interface
- Invoice generation
- Payment processing
- Daily sales tracking

## 🤝 Contributing

1. 🍴 Fork the repository
2. 🌿 Create feature branch (`git checkout -b feature/new-feature`)
3. 💾 Commit changes (`git commit -m 'Add new feature'`)
4. 📤 Push to branch (`git push origin feature/new-feature`)
5. 🔄 Create Pull Request


## 📄 License

📜 MIT License - see [LICENSE](LICENSE) file for details.

- 📖 **Documentation**: [Project Wiki](https://github.com/AmashaUdugama/Cosmatic-Shop/wiki)

---

⭐ **Star this repo if you find it helpful!** ⭐

**Made with ❤️ for cosmetic shop management**
