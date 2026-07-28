# 🗺️ Tourist Guide System

A full-featured Dynamic Web Application built with Java Servlets, JSP, JDBC, MySQL, and Apache Tomcat. The Tourist Guide System allows users to explore tourist destinations, search places, view interactive details, and send feedback, while providing administrators with a dashboard to manage destinations, users, and queries.

---

## 📸 Application Screenshots & UI Showcase

### 🖥️ Main Dashboard & Platform Screenshots
| Home / Index View | Search Destinations |
| :---: | :---: |
| ![Application Screen](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image13.png) | ![Search Place](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image14.png) |

| Tourist Place Details | User Login & Captcha |
| :---: | :---: |
| ![Place Details](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image15.png) | ![User Login](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image16.png) |

| User Registration | User Dashboard |
| :---: | :---: |
| ![User Registration](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image17.png) | ![User Dashboard](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image18.png) |

| Admin Login | Admin Dashboard |
| :---: | :---: |
| ![Admin Login](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image19.png) | ![Admin Dashboard](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image20.png) |

| Add Tourist Place | View Feedback & Q&A |
| :---: | :---: |
| ![Add Tourist Place](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image21.png) | ![Feedback View](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image22.png) |

---

## 📊 System Architecture & Data Flow Diagrams (DFD)

### 👤 User Data Flow Diagram
![User DFD](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image1.png)

### 🛡️ Admin Data Flow Diagram
![Admin DFD](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image2.png)

---

## 🗄️ Database Tables & Schema Overview

| Admin Table | User Table | Tourist Place Table |
| :---: | :---: | :---: |
| ![Admin Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image5.jpeg) | ![User Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image10.jpeg) | ![Tourist Place Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image9.jpeg) |

| Feedback Table | Contact Table | Questions & Answers Table |
| :---: | :---: | :---: |
| ![Feedback Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image8.jpeg) | ![Contact Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image7.JPG) | ![Questions Table](TouristGuideSystem/WebContent/assets/images/doc_screenshots/image11.jpeg) |

---

## 🏞️ Destination Showcase & Photos

| Goa | Kerala | Jammu & Kashmir |
| :---: | :---: | :---: |
| ![Goa](TouristGuideSystem/WebContent/images/goa.jpg) | ![Kerala](TouristGuideSystem/WebContent/images/kerala.jpg) | ![Jammu & Kashmir](TouristGuideSystem/WebContent/images/jammu-kashmir.jpg) |

| Himachal Pradesh | Mahabaleshwar | Dynamic Uploads |
| :---: | :---: | :---: |
| ![Himachal Pradesh](TouristGuideSystem/WebContent/images/himachal.png) | ![Mahabaleshwar](TouristGuideSystem/WebContent/upload/mahabaleshwar.jpg) | ![Kerala Upload](TouristGuideSystem/WebContent/upload/kerala.jpg) |

---

## 🧳 Tourism Services & Amenities

| Service | Service | Service |
| :---: | :---: | :---: |
| ![Airport Transfers](TouristGuideSystem/WebContent/images/airport-transfers.jpg)<br>**✈️ Airport Transfers** | ![Car Rentals](TouristGuideSystem/WebContent/images/car-rentals.jpg)<br>**🚗 Car & Cab Rentals** | ![Hotel Booking](TouristGuideSystem/WebContent/images/hotel-compensession.jpg)<br>**🏨 Hotel & Stay Guarantees** |
| ![Train Booking](TouristGuideSystem/WebContent/images/trains.jpg)<br>**🚆 Train Travel** | ![24/7 Support](TouristGuideSystem/WebContent/images/customer-support.jpg)<br>**🎧 24/7 Customer Support** | ![Best Price Guarantee](TouristGuideSystem/WebContent/images/price.jpg)<br>**🏷️ Best Price Guarantee** |

---

## 🌟 Key Features

### 👤 User Module
- **Registration & Login**: Secure user authentication with password encryption (AES) and CAPTCHA validation.
- **Search Destinations**: Search tourist locations by keyword, place, or category.
- **Place Details & Maps**: View location details, high-resolution photos, and interactive map guidance.
- **Feedback & Support**: Submit feedback and ask questions via interactive forms.

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
│   │   ├── assets/images/           
│   │   │   └── doc_screenshots/     # Screenshots extracted from project documentation
│   │   ├── images/                  # Tourist destination photos & banners
│   │   └── upload/                  # User & admin uploaded place photos
│   ├── .classpath                   # Eclipse project classpath configuration
│   └── .project                     # Eclipse project definition
├── .gitignore                       # Git ignore file
├── LICENSE                          # MIT License
└── README.md                        # Project documentation with photos & DFD diagrams
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
