# Smart Student Management System (Python)

A simple, beginner-friendly **Student Management System** built with core Python — no external libraries, no frameworks. Great for learning fundamentals: functions, dictionaries, lists, file I/O, and JSON/CSV handling.

## Features

- **Add Student** – Create a new student record (auto roll number or custom)
- **Update Student** – Edit name, age, or department
- **Delete Student** – Remove a record with confirmation
- **Search Student** – Search by roll number or partial name match
- **Display All Students** – View every record with marks, grade, and attendance
- **Calculate Grades** – Enter subject-wise marks and auto-calculate average + letter grade
- **Attendance Management** – Mark present/absent by date, view attendance %
- **Data Storage** – All data saved in `students.json` (auto-loads on startup)
- **Login System** – Simple username/password authentication (`users.json`)
- **Export Reports** – Generate:
  - Individual student report card (`.txt`)
  - All students summary (`.csv`)
  - Class-wide grade distribution summary (`.txt`)

## Requirements

- Python 3.7 or higher
- No external packages needed (uses only `json`, `os`, `csv`, `datetime` from the standard library)

## How to Run

```bash
python3 student_management.py
```

On first run, a default login is created automatically:

```
Username: admin
Password: admin123
```

You can also register a new user from the start menu.

## Grading Scale

| Average Marks | Grade | Remark             |
|----------------|-------|---------------------|
| 90 – 100       | A     | Excellent           |
| 75 – 89        | B     | Very Good           |
| 60 – 74        | C     | Good                |
| 40 – 59        | D     | Needs Improvement   |
| Below 40       | F     | Fail                |

## Project Structure

```
.
├── student_management.py   # Main program (single file)
├── students.json            # Auto-created — stores student records
├── users.json                # Auto-created — stores login credentials
├── reports/                   # Auto-created — exported reports land here
└── README.md
```

## Notes

- This project stores passwords in plain text inside `users.json` for simplicity. It is meant for **learning purposes only** — do not reuse this login system for real applications.
- `students.json` and `users.json` are created automatically the first time you run the program, so the repo ships without them.

## Possible Extensions

- Add password hashing (e.g. with `hashlib`)
- Add input validation for age/marks ranges
- Add a GUI using `tkinter`
- Add sorting/filtering options in "Display All Students"
