# Online School Management System

A comprehensive web-based school management system built with PHP that handles tests, classes, students, and teachers management.

## Features

- User Management (Students, Teachers, Administrators)
- Class Management
- Test Creation and Management
- Test Taking and Marking
- PDF Generation for Test Results
- School Management (Multi-school Support)
- Profile Management
- Authentication System

## Technology Stack

- **Backend:** PHP (Custom MVC Framework)
- **Database:** MySQL/MariaDB
- **Frontend:** Bootstrap 5.0.2
- **Icons:** Font Awesome 5.15.2
- **PDF Generation:** mPDF

## System Requirements

- PHP 8.0.3 or higher
- MySQL/MariaDB 10.4.18 or higher
- Apache Web Server
- XAMPP (recommended)

## Database Structure

The system uses a MySQL database with the following main tables:

- `users` - Stores user information
- `schools` - Manages school data
- `classes` - Handles class information
- `tests` - Stores test data
- `test_questions` - Contains test questions
- `answers` - Stores student answers
- `answered_tests` - Tracks completed tests
- `class_lecturers` - Maps teachers to classes
- `class_students` - Maps students to classes

## Directory Structure

```
├── private/
│   ├── controllers/     # Application controllers
│   ├── core/           # Framework core files
│   ├── models/         # Data models
│   └── views/          # View templates
├── public/
│   ├── assets/         # Static assets
│   ├── generated_pdfs/ # Generated test results
│   ├── uploads/        # User uploads
│   └── index.php       # Entry point
└── school_db.sql       # Database schema
```

## Installation

1. Install XAMPP with PHP 8.0.3 or higher
2. Clone this repository to your htdocs folder
3. Import `school_db.sql` to create the database
4. Configure database connection in `private/core/config.php`
5. Access the application through your web browser

## Key Features Details

### User Management
- Multiple user roles (students, teachers, administrators)
- Profile management
- School switching capability for users in multiple schools

### Class Management
- Create and manage classes
- Assign teachers and students
- Track class activities and tests

### Test System
- Create various types of tests (objective, multiple choice)
- Automatic and manual grading
- PDF generation of test results
- Test statistics and analysis

### School Management
- Multi-school support
- School-specific user management
- School-specific class management

## Security Features

- Password hashing
- Session management
- Access control based on user roles
- Input validation and sanitization

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

## License

This project is open-source and available under the MIT License.

