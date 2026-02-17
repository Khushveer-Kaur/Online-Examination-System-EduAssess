# Online-Examination-System-EduAssess

EduAssess is a secure AI-assisted online examination platform designed to conduct fair remote assessments.  
The system enables teachers to create exams, students to attempt them, and administrators to monitor and manage the platform (while preventing cheating using automated proctoring and rule enforcement).

It supports real-time monitoring, automatic grading, attempt control, and structured database-driven evaluation.

---

## Project Objective
Traditional online exams suffer from cheating, impersonation, and lack of monitoring.  
EduAssess solves this by combining:

- Authentication + role based access
- Anti-cheating monitoring
- Auto grading
- Attempt restrictions
- Centralized database evaluation

The system provides a controlled and secure digital exam environment suitable for universities, coaching institutes, and training programs.

---

## Tech Stack

**Backend**
- Python

**Frontend**
- HTML
- CSS
- JavaScript

**Database**
- Oracle Database (SQL + PL/SQL)

---

## Prerequisites

- Python 3.8+
- Oracle Database (Express Edition or higher)
- requirements.txt

## Database Setup

### Step 1: Install Oracle Database

Download and install Oracle Database XE from:
https://www.oracle.com/database/technologies/xe-downloads.html

### Step 2: Run SQL Schema

1. Open SQL Developer
2. Connect to your Oracle database
3. Open the file `DB.sql`
4. Run all the SQL commands (F5)

### Step 3: Create Database User
```sql
-- Connect as SYSTEM
CREATE USER C##exam_admin IDENTIFIED BY exam_password_123;
GRANT CONNECT, RESOURCE, DBA TO C##exam_admin;
GRANT UNLIMITED TABLESPACE TO C##exam_admin;
COMMIT;
```

## Running the APP
1. Run main.py (runs the backend)
2. Run login.html (runs the frontend)
