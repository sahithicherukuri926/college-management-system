# college-management-system
Overview

The College Management System is a Python-based application designed to manage colleges, students, and teachers efficiently. It enables administrators to create colleges, add teachers and students, and securely display their details using OTP (One-Time Password) verification. The system provides a simple menu-driven interface for interaction and uses email-based OTP authentication for secure access control.

Key Features

Create Colleges: Assigns unique IDs and names to colleges.

Add Teachers: Add teachers with subject specialization, email, and OTP-based verification.

Add Students: Register students with their branch and email, secured by OTP verification.

Display Teacher and Student Details: View details of teachers and students associated with a college, accessible only after OTP verification.

Secure OTP Verification: Ensures that only authorized users can access sensitive information.

Technologies Used

Python 3.x: Main programming language used for development.

smtplib: Used for sending OTP verification emails to users.

email.mime: Utilized for formatting OTP emails.

random: Generates random OTPs for user verification.

Requirements

To run the system, ensure you have the following:

Python 3.x installed

Built-in Python libraries:

smtplib

email.mime

A valid email account configured for sending OTPs

If additional dependencies are required, they can be installed using a requirements.txt file.

How It Works

1. Create College

Input a unique college ID and name to create a new college.

2. Add Teacher

Input the college ID, teacher’s name, email, and subject specialization.

An OTP will be sent to the teacher’s email for verification.

After successful OTP verification, the teacher will be added to the system.

3. Add Student

Input the college ID, student’s name, email, and branch.

An OTP will be sent to the student’s email for verification.

After successful OTP verification, the student will be added to the system.

4. Display Teacher/Student Details

Input the college ID to view details of teachers or students associated with that college.

Access will be granted only after successful OTP verification.

5. Exit

The user can exit the program at any time.

Example of OTP Email

When adding a teacher or student, an email will be sent with the following format:

Subject: College Management System - OTP Verification

Dear [User],

Your OTP for verification is: [XXXXXX]

Please enter this OTP to complete your registration.

Thank you.

After receiving the OTP, the user will be prompted to enter the code for verification. If the OTP is correct, the teacher or student will be successfully added to the system.

Security Considerations

Use a dedicated email account for sending OTPs in a production environment.

Do not hard-code sensitive information (e.g., email credentials) in the source code. Instead, use environment variables or a configuration file for secure credential management.

Future Improvements

Database Integration: Store data persistently using a database (e.g., SQLite, MySQL).

Graphical User Interface (GUI): Develop a user-friendly GUI.

SMS OTP Support: Implement OTP verification via SMS using services like Twilio.

Role-Based Access Control: Introduce different user roles for administrators, teachers, and students.
