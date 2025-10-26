# 🏨 Hotel Reservation System

A simple Java-based hotel management application using MySQL.

## ⚙️ Features
- Reserve a room
- View reservations
- Update or delete reservations
- JDBC + MySQL integration

## 🧰 Requirements
- Java 21+
- MySQL Server
- MySQL Connector/J 8.4.0

## 🚀 Run Instructions
1. Import project in IntelliJ.
2. Add MySQL Connector/J in classpath.
3. Run `HotelReservationSystem.java`.

## 📦 Database Setup
```sql
CREATE DATABASE hotel_db;
USE hotel_db;
CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(50),
    room_number INT,
    contact_number VARCHAR(15),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
