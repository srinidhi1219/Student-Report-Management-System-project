# Student-Report-Management-System-project
A Student Report Management System is a software application used to store, manage, and generate student academic records such as marks and grades. It reduces manual work and helps in quick, accurate report handling..

# Student Report Management System

A console-based Student Report Management System built in C for managing student records through a simple role-based interface.

## Overview

This project is a file-based student record management application developed as a college project. Users log in based on their role and get access only to the operations available for that role — like viewing, searching, or managing student records. Student data is stored locally using text files instead of a database.

## Features

- Role-based login for Admin, Staff, and Guest users
- Add student records
- Display student records
- Search for student records
- Update student information
- Delete student records (Admin only)
- Different menu options depending on the logged-in role

## Tech Stack

- C
- File Handling (stdio.h)
- GCC Compiler

## How It Works

The application starts with a login screen where the user enters a username and password. Once authenticated, the menu shown depends on the user's role:

- **Admin** – Add, Display, Search, Update, Delete
- **Staff** – Add, Display, Search, Update (no delete access)
- **Guest** – Display and Search only (read-only)

Student records are stored in `students.txt` and read from there whenever the program runs.

## How to Run

Make sure a C compiler such as GCC/MinGW is installed.

```bash
gcc "CCC code.cpp" -o student_report
./student_report
```

## Project Structure

```
├── CCC code.cpp       # Main source code
├── students.txt        # Stores student records
├── credentials.txt     # Demo login credentials (see below)
└── README.md
```

## Login Credentials

The repo includes a demo credentials file (`credentials.txt`) with sample admin, staff, and guest logins used to test the role-based access system. These are dummy values for demonstration only — not real or secure credentials.

## Notes

Built as a college coursework project to practice file handling and role-based access logic in C. Data is stored in plain text for simplicity — not intended for production use.

## Future Improvements

- Support student names containing spaces (currently limited to single-word names)
- Add input validation for roll numbers and marks
- Migrate storage to SQLite for better data integrity
- Add password hashing instead of storing credentials in plain text
```

Just paste that whole thing directly into your README.md on GitHub, replacing whatever's there now.
