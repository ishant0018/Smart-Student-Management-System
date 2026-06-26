
# Student Management System (Python)

A simple console-based Student Management System built with core Python. Stores records in a local JSON file — no external libraries required.

## Features

- **Add Student** — roll number, name, age, course, marks (auto-calculates grade)
- **Display All Students** — view every saved record
- **Search Student** — look up a student by roll number
- **Update Student** — edit any field, leave blank to keep existing value
- **Delete Student** — remove a record by roll number
- **Persistent Storage** — all data saved to `students.json`, reloaded automatically on startup

## Grading Scale

| Marks      | Grade |
|------------|-------|
| 90 – 100   | A+    |
| 80 – 89    | A     |
| 70 – 79    | B     |
| 60 – 69    | C     |
| Below 60   | F     |

## Requirements

- Python 3.x
- No external packages (only built-in `json` and `os` modules)

## How to Run

```bash
python3 student_management.py
```

## Project Structure

```
.
├── student_management.py   # Main program
├── students.json             # Auto-created on first run (stores records)
├── README.md
└── .gitignore
```

## Notes

`students.json` is created automatically the first time you add a student, so the repository starts empty.
