# University Training Database

## 📋 Description

A complete relational database project for learning SQL and Data Engineering
concepts as part of the AI Data Engineering training path.

## 🗂️ Project Structure

## 🗃️ Database Tables

| Table | Description |
|-------|-------------|
| `students` | Student information |
| `courses` | Course information |
| `instructors` | Instructor information |
| `enrollments` | Student-course enrollments |
| `assessments` | Student scores per course |

## 🔗 Relationships

- Students **1:N** Enrollments
- Courses **1:N** Enrollments
- Instructors **1:N** Courses
- Students **1:N** Assessments
- Courses **1:N** Assessments

## 🛠️ Technologies

- **SQLite** — Lightweight local database
- **PostgreSQL** — Server-based RDBMS
- **SQL** — Query language
- **Python 3** — Data extraction
- **Pandas** — Data manipulation
- **Git / GitHub** — Version control

## 🚀 Getting Started

```bash
# 1. Create database
sqlite3 database/university.db < database/schema.sql
sqlite3 database/university.db < database/seed.sql

# 2. Run queries
sqlite3 database/university.db < queries/basic_queries.sql
sqlite3 database/university.db < queries/joins.sql
sqlite3 database/university.db < queries/reports.sql

# 3. Extract data to CSV
python python/extract_data.py