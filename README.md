#  SQL Database Project - Student Management System

This project showcases my ability to design a relational database for managing students, their departments, semesters, courses, and grades using SQL.  
It demonstrates how to build a normalized schema, insert realistic data, and perform analytical queries.

## Description

The project includes:
- Creating multiple related tables: Student, Department, Course, Semester, StudyYear, and Marks
- Defining primary and foreign key relationships
- Inserting sample data (at least 5 students and their marks)
- Adding constraints such as `CHECK (Mark BETWEEN 0 AND 100)`
- Using `JOIN`, `GROUP BY`, and aggregate functions like `AVG` and `COUNT` to analyze student performance

## Technologies Used
- SQL (Oracle)
- SQL*Plus

##  Sample Query

```sql
-- Display student names with their course and mark
SELECT Student.STName, Course.CoName, STMark.MarkVal
FROM STMark
JOIN Student ON STMark.STNo = Student.STNo
JOIN Course ON STMark.CoNo = Course.CoNo;

## About Me
This project was created during my training in the Makeen Bootcamp.
It reflects my understanding of database design principles, normalization, and the ability to use SQL for managing educational data.
