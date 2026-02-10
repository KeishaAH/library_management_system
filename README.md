# Library Management System – MySQL Database Project

## Project Overview
This project is a **Library Management System Database** developed using **MySQL**.  

The system is designed to manage:
- Library catalog and knowledge resources
- Users (Students & Lecturers)
- Librarians
- Borrow, Return, and View transactions
- Payments and fines
- Notifications for overdue resources

---

## Objectives
- To design and implement a relational database for a university library.
- To manage borrowing, returning, and overdue penalties automatically.
- To demonstrate database concepts such as triggers, constraints, and relationships.

---

## Features

### 1. Catalog Management
- Store physical and digital resources.
- Categorize by title, subject, author, publisher, and rack location.
- Support unlimited digital content quantity.

### 2. User Management
- Student and Lecturer roles.
- Account details, gender, DOB, department, and major.
- Restriction system for overdue or unpaid fines.

### 3. Transaction System
- Borrow, Return, and View actions.
- Automatic due date generation.
- Late and damage/lost status tracking.

### 4. Payment & Fine Management
- Automatic fine calculation.
- Purchase and fine payment methods.
- Invoice generation.

### 5. Notification System
- Overdue day tracking.
- Fine notification for users.

---

## Database Structure

### Main Tables
- `Rack`
- `Author`
- `Publisher`
- `KnowledgeResource`
- `User`
- `Librarian`
- `Transaction`
- `Payment`
- `Notification`

---

## Triggers Implemented
- **CombinedTransactionTrigger**
  - Restricts banned users from borrowing.
  - Sets due date automatically.
  - Calculates overdue price and status.

- **CopyBookPriceToPurchasePrice**
  - Copies book price into payment purchase price.

- **AutoGeneratePaymentAndNotificationAfterReturn**
  - Generates invoice and notification automatically after return.

---

## Technologies Used
- MySQL
- SQL Triggers
- Relational Database Design
- ERD / EERD Concepts

---

## How to Run

1. Open **MySQL Workbench** or **phpMyAdmin**
2. Import the file: library_management_system.sql
3. Execute the script.
4. The database and all tables will be created automatically.

---

## Sample Data
The project includes:
- 15 Users
- 5 Librarians
- 38 Knowledge Resources
- Multiple transactions, racks, authors, and publishers.

---

## Learning Outcomes
- Entity Relationship Modeling
- SQL Table Design
- Constraints & Foreign Keys
- Triggers & Automation
- Transaction Management

---
