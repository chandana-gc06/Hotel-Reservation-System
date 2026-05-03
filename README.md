# Hotel Reservation System

A Java-based hotel management system for managing room reservations using MySQL database.

## Features

- Reserve a room
- View reservations
- Get room number
- Update reservations
- Delete reservations

## Prerequisites

- Java JDK 8 or higher
- MySQL Server
- MySQL Connector/J (mysql-connector-j-9.6.0.jar)

## Setup

1. Create MySQL database and table:

   CREATE DATABASE hotel_db;
   USE hotel_db;
   CREATE TABLE reservations (
       reservation_id INT AUTO_INCREMENT PRIMARY KEY,
       guest_name VARCHAR(100),
       room_number INT,
       contact_number VARCHAR(15),
       reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );

2. Set environment variables:

   set DB_URL=jdbc:mysql://localhost:3306/hotel_db
   set DB_USERNAME=root
   set DB_PASSWORD=your_password

3. Compile & Run
   javac -cp ".;mysql-connector-j-9.6.0.jar" HotelReservationSystem.java
   java -cp ".;mysql-connector-j-9.6.0.jar" HotelReservationSystem

   
