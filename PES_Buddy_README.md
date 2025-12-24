
# PES Buddy

PES Buddy is a **console-based campus utility application** developed in **C**, designed to assist university students with common on-campus tasks such as expense management, scooter booking, and canteen food ordering.

---

## Table of Contents
- Overview
- Features
- System Design
- Project Structure
- Installation & Execution
- Usage Guide
- Technologies Used
- Future Enhancements
- License

---

## Overview

PES Buddy integrates multiple student-oriented services into a single menu-driven program.  
The project focuses on applying fundamental **C programming concepts** to build a modular, real-world inspired application suitable for academic evaluation.

The system runs entirely on the command line and uses file handling for data persistence.

---

## Features

### User Authentication
- User registration and login system
- SRN-based authentication
- User data stored in `users.txt`
- Limited login attempts for basic security

### Expense Tracker
- Weekly expense tracking
- Supports up to four categories:
  - Food
  - Travel
  - Study Materials
  - Miscellaneous
- Weekly expense summary
- Category-wise expense analysis
- Alerts when the weekly spending limit is exceeded

### PES Scootigo – Scooter Booking System
- Displays available scooters with driver details
- Allows booking between predefined campus locations:
  - GJBC ↔ OAT
  - SKM ↔ BE Block
  - MRD Block ↔ F Block
- Calculates total fare based on distance and per-kilometer cost
- Prevents duplicate bookings

### PES Doormato – Food Ordering System
- Food ordering from multiple campus canteens
- Dynamic menu loading from text files
- Maintains order summary and total cost
- Supports multiple item orders from different canteens

---

## System Design

- Menu-driven architecture using switch-case
- Modular functions for each feature
- Structures used to manage orders
- File handling for user and menu data
- Input validation for better reliability

---

## Project Structure

```
.
├── PesBuddy.c
├── users.txt
├── skm_menu.txt
├── gjbc_menu.txt
├── bebloc_menu.txt
├── hornbill_menu.txt
└── README.md
```

---

## Installation & Execution

### Prerequisites
- GCC Compiler
- Linux / macOS / Windows (with GCC installed)

### Compile
```bash
gcc PesBuddy.c -o PesBuddy
```

### Run
```bash
./PesBuddy
```

---

## Usage Guide

1. Register a new user or login using SRN credentials
2. Access the main menu
3. Select one of the available services:
   - Expense Tracker
   - PES Scootigo
   - PES Doormato
4. Follow on-screen instructions
5. Exit or return to the main menu

---

## Technologies Used
- Programming Language: C
- Core Concepts:
  - Structures
  - File Handling
  - Arrays and Strings
  - Modular Programming
  - Menu-driven Design

---

## Future Enhancements
- Password encryption
- Database integration
- Graphical user interface
- Improved error handling
- Real-time data persistence

---

## License

This project is developed strictly for **educational purposes**.
