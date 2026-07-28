# 🗺️ Tourist Guide System

A full-featured Dynamic Web Application built with Java Servlets, JSP, JDBC, MySQL, and Apache Tomcat. The Tourist Guide System allows users to explore tourist destinations, search places, view interactive details, and send feedback, while providing administrators with a dashboard to manage destinations, users, and queries.

---

## 📸 Screenshots & System Preview

### 🖥️ User Dashboard & Interface
![User Dashboard](TouristGuideSystem/WebContent/assets/images/user-dashboard.png)

### 🌐 System Overview
![Intelligent Tourism System Overview](TouristGuideSystem/WebContent/assets/images/intelligent-tourism-system.jpg)

---

## 🏞️ Featured Tourist Destinations

| Destination | Destination | Destination |
| :---: | :---: | :---: |
| ![Goa](TouristGuideSystem/WebContent/images/goa.jpg)<br>**Goa** | ![Kerala](TouristGuideSystem/WebContent/images/kerala.jpg)<br>**Kerala** | ![Jammu & Kashmir](TouristGuideSystem/WebContent/images/jammu-kashmir.jpg)<br>**Jammu & Kashmir** |
| ![Himachal Pradesh](TouristGuideSystem/WebContent/images/himachal.png)<br>**Himachal Pradesh** | ![Airport Transfers](TouristGuideSystem/WebContent/images/airport-transfers.jpg)<br>**Airport Transfers** | ![Car Rentals](TouristGuideSystem/WebContent/images/car-rentals.jpg)<br>**Car Rentals** |

---

## 🌟 Key Features

### 👤 User Module
- **Registration & Login**: Secure user authentication and profile management.
- **Search Destinations**: Search tourist locations by keyword, place, or category.
- **Place Details & Maps**: View location details, high-resolution photos, and map guidance.
- **Feedback & Support**: Submit feedback and ask questions via interactive forms with CAPTCHA verification.

### 🛡️ Admin Module
- **Admin Dashboard**: Overview of key platform metrics.
- **Manage Tourist Places**: Add, edit, update, or remove tourist spots and upload destination images.
- **Manage Users**: View registered users and platform user activity.
- **Feedback & Inquiries**: Review user feedback and messages.

---

## 🛠️ Technology Stack

| Layer | Technology |
|---|---|
| **Frontend** | HTML5, CSS3, JavaScript, JSP (JavaServer Pages) |
| **Backend** | Java (JDK 8+), Servlets, JDBC |
| **Database** | MySQL Server 8.0+ |
| **Server Runtime** | Apache Tomcat 8.5 / 9.0+ |
| **IDE Support** | Eclipse Enterprise Java / IntelliJ IDEA / NetBeans |

---

## 📁 Repository Structure

```
Tourist Guide System + Database/
├── Database/
│   └── tourist_guide_system.sql     # Database dump & schema
├── TouristGuideSystem/
│   ├── src/                         # Java source files (Servlets, Connection, Logic)
│   ├── WebContent/                  # Web assets (JSPs, CSS, JS, Images, WEB-INF)
│   │   ├── assets/images/           # System screenshots & dashboard previews
│   │   └── images/                  # Tourist destination photos & banners
│   ├── .classpath                   # Eclipse project classpath configuration
│   └── .project                     # Eclipse project definition
├── .gitignore                       # Git ignore file
├── LICENSE                          # MIT License
└── README.md                        # Project documentation with photos
```

---

## 🚀 Getting Started & Installation

### Prerequisites
Ensure you have the following installed on your system:
- **Java Development Kit (JDK 8 or higher)**
- **Apache Tomcat Server (v8.5 or v9.0 recommended)**
- **MySQL Database Server (v5.7 or v8.0)**
- **Eclipse IDE for Enterprise Java Developers** (or equivalent IDE)

---

### 1. Database Setup
1. Open your MySQL client (e.g., MySQL Workbench, phpMyAdmin, or command line).
2. Create a new database named `tourist_guide_system`:
   ```sql
   CREATE DATABASE tourist_guide_system;
   ```
3. Import the database schema from the `Database` folder:
   ```bash
   mysql -u root -p tourist_guide_system < Database/tourist_guide_system.sql
   ```

---

### 2. Configure Database Credentials
Verify or update the MySQL database connection settings in Java:
- Path: `TouristGuideSystem/src/com/connection/DatabaseConnection.java`
- Lines 18–19:
  ```java
  Class.forName("com.mysql.cj.jdbc.Driver");
  connection = DriverManager.getConnection("jdbc:mysql://localhost/tourist_guide_system?useSSL=false", "YOUR_DB_USER", "YOUR_DB_PASSWORD");
  ```

---

### 3. Deploy & Run the Application

#### Using Eclipse IDE:
1. Open Eclipse and select **File > Import...**
2. Choose **Existing Projects into Workspace** and browse to the `TouristGuideSystem` folder.
3. Add **Apache Tomcat** as your Target Runtime in project properties.
4. Right-click the project -> **Run As > Run on Server**.
5. Access the application in your browser at:
   ```
   http://localhost:8080/TouristGuideSystem/
   ```

---

## 🔑 Default Credentials

- **Admin Portal**: Accessible via `/admin-login.jsp`
  - **Username**: `admin`
  - **Password**: `admin` *(or password initialized in `tbladmin`)*

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
