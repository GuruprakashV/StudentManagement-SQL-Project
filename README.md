# StudentManagement-SQL-Project
A student project to design a `StudentManagement` database, create tables with constraints, and execute SQL queries to manage students, courses, enrollments, and instructors effectively.

Objective
The goal of this project is for students to design a database, create tables with appropriate data types and constraints, and perform various SQL operations based on provided questions.

Project Overview
This project involves setting up a StudentManagement database to manage student records, course information, enrollments, and instructor assignments. Students will gain hands-on experience in database design, table creation, and executing SQL queries to solve real-world problems.

Database Schema
Tables
Students

Columns:
student_id (INT): Primary Key, Auto-incremented.
first_name (VARCHAR 50): Not Null.
last_name (VARCHAR 50): Not Null.
date_of_birth (DATE): Not Null.
gender ('Male', 'Female', 'Other'): Not Null.
email (VARCHAR 100): Unique, Not Null.
phone_number (VARCHAR 15): Unique.
address (TEXT).
Courses

Columns:
course_id (INT): Primary Key, Auto-incremented.
course_name (VARCHAR 100): Not Null.
course_description (TEXT).
credit_hours (INT): Not Null.
Enrollment

Columns:
enrollment_id (INT): Primary Key, Auto-incremented.
student_id (INT): Foreign Key referencing Students(student_id).
course_id (INT): Foreign Key referencing Courses(course_id).
enrollment_date (DATE): Not Null.
Instructors

Columns:
instructor_id (INT): Primary Key, Auto-incremented.
first_name (VARCHAR 50): Not Null.
last_name (VARCHAR 50): Not Null.
email (VARCHAR 100): Unique, Not Null.
phone_number (VARCHAR 15): Unique.
CourseAssignments

Columns:
assignment_id (INT): Primary Key, Auto-incremented.
course_id (INT): Foreign Key referencing Courses(course_id).
instructor_id (INT): Foreign Key referencing Instructors(instructor_id).
SQL Queries
Students are required to answer the following questions using SQL queries:

Retrieve the full names and email addresses of all students enrolled in the Computer Science course.
List all courses along with the number of students enrolled in each course.
Find the instructors who are teaching more than 2 courses.
Retrieve the details of students (name, email) who are enrolled in a course taught by a specific instructor.
List all students who have not enrolled in any course.
Get the list of courses with no assigned instructor.
Retrieve the full details of the Students table, sorted by last name.
Find the total number of credit hours for a student enrolled in specific courses.
Identify the student with the maximum number of enrollments.
Get the details of students whose phone numbers are missing.
