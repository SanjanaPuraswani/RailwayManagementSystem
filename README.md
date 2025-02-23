# Railway Management System

## 📌 Project Overview
The **Railway Management System** is a desktop application built using **Java** with **JDBC** for database connectivity and a **GUI** interface developed using **Swing** (or **JavaFX**, if applicable). The system manages railway operations such as passenger reservations, train schedules, ticket bookings, and more.

## 🛠️ Features

### User Module
- User registration and login
- Ticket booking and cancellation
- View train schedules
- Check booking history

### Admin Module
- Add, update, and delete train information
- Manage train schedules
- View all reservations and user details

### System Features
- Secure authentication system
- Search functionality for trains
- Error handling and input validation
- Interactive and user-friendly GUI

## 🗂️ Technology Stack

- **Language**: Java
- **Database**: MySQL (or any JDBC-supported RDBMS)
- **Frameworks/Tools**: JDBC, Swing/JavaFX
- **IDE**: IntelliJ IDEA / Eclipse / NetBeans

## 📋 Requirements

Ensure the following are installed:

- Java Development Kit (JDK 17 or higher)
- MySQL Server
- IDE (IntelliJ IDEA, Eclipse, or any preferred Java IDE)

## 🏗️ Setup Instructions

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/railway-management-system.git
   cd railway-management-system
   ```

2. **Configure the database:**

   - Create a MySQL database:
     ```sql
     CREATE DATABASE railway_management;
     ```
   - Import the provided SQL schema:
     ```bash
     mysql -u your-username -p railway_management < database/schema.sql
     ```

3. **Update database credentials:**

   Ensure the correct MySQL credentials are set in the Java code:

   ```java
   String url = "jdbc:mysql://localhost:3306/railway_management";
   String username = "your-username";
   String password = "your-password";
   ```

4. **Compile and run the application:**

   ```bash
   javac src/*.java
   java src.Main
   ```

## 📊 Database Schema

**Tables:**

1. `users` - Stores user details (user_id, username, password, role)
2. `trains` - Stores train information (train_id, name, source, destination, departure_time)
3. `passengers` - Stores passenger details (passenger_id, name, age, gender, contact_number)
4. `trips` - Stores trip details (trip_id, train_id, departure_station, arrival_station, trip_date)
5. `staff` - Stores staff information (staff_id, name, role, contact_number)
6. `stations` - Stores station details (station_id, station_name, location)
7. `reservations` - Stores ticket bookings (reservation_id, user_id, train_id, seat_number)

## 🧪 Sample Credentials

- **Admin**: admin / admin123
- **User**: user / user123

## 📸 Screenshots

1. Login Page
2. User Dashboard
3. Admin Panel
4. Ticket Booking Page

## 🤝 Contribution Guidelines

Contributions are welcome!

1. Fork the repository
2. Create a new branch
3. Make your changes
4. Submit a pull request

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

🚀 **Enjoy building and managing the Railway System!**

