# rhombic_technologies_tasks_02
Student Grade Management System

## Description

The Grade Tracker System is an academic management tool designed for both students and teachers. This system allows students to view their grades, while teachers can manage student information, grades, attendance, and portfolios. The system stores the academic data in an Excel file and supports CRUD operations for managing student grades and other academic records.

### Key Features:
- **Student Functions:**
  - View grades for subjects.
  - View attendance (future feature).
  - View portfolio (future feature).
  
- **Teacher Functions:**
  - Add new students.
  - Add or update student grades.
  - Delete student grades.
  - Mark attendance for students.
  - Add portfolio entries for students.
  - List all students.
  - View detailed student information.
  - Calculate the average grade for all students.

### Technologies Used:
- Python 3.x
- `openpyxl` library for Excel file manipulation.
- Password hashing for secure user authentication.

## Getting Started

### Prerequisites:
1. Install Python 3.x (if not already installed).
2. Install the required Python libraries using `pip`:
   ```bash
   pip install openpyxl
   
###Limitations
Attendance and Portfolio Features:

The attendance and portfolio features are placeholders and not fully implemented yet. The system prints a message stating that the functionality is not implemented.
Input Format for Grades:

Grades should be entered as individual numeric values (e.g., 3.5). If you input comma-separated values like 3.1, 2.3, 3.3 in a grade cell, the program will split and calculate the average grade, but this is not the ideal way to input grades. Multiple grades per subject should ideally be stored in separate rows, not in a single cell.
Password Storage:

Passwords are stored as SHA-256 hashes, which is a more secure approach than storing them as plain text. However, the security could be improved by integrating a more robust authentication system, such as bcrypt or using an external library for handling password storage.
Excel File Corruption:

If the Excel file (grades.xlsx) is corrupted or not in the correct format, the program may fail to read the file. Always ensure the file is properly structured and saved before running the program.
Data Validation:

The system doesn't currently handle more complex data validation. For example, it doesn't check if the student ID is unique when adding new students or whether the grade input is within a valid range (e.g., 0-100).
No GUI:

This system is command-line-based and does not include a graphical user interface (GUI). If you're looking for a more user-friendly interface, additional work would be needed to implement one.

