# Machine Maintenance Monitoring System

## Project Description
This project is a simple Python-based data management system designed to store, read, validate and summarise machine maintenance records.

It demonstrates basic Python concepts such as file handling, regular expressions, functions, dictionaries and report generation.

## Data Format
The dataset is stored in `data/sample.txt`.

Each record contains four comma-separated fields:

- **Machine_ID:** Unique machine identification.
- **Temperature:** Machine temperature in °C.
- **Pressure:** Machine pressure in bar.
- **Status:** Operating condition (ON/OFF).

**Example Record:**
`M01,75,5.2,ON`

## Project Structure

```text
Project/
│
├── data/
│   └── sample.txt
│
├── reports/
│
├── datalayer.py
│
├── main.py
│
└── README.md
```

## Jobs Completed

### JOB A – Real Data, Written by Hand
Created a dataset containing 15 manually entered machine records, including three intentionally imperfect records:
- Extra spaces
- Missing field
- Out-of-range temperature

### JOB B – Read, Validate and Report
Created three functions in `datalayer.py`:
- `parse_record()` – Validates and converts a record into a dictionary.
- `load()` – Reads the file and separates valid records from problems.
- `summarise()` – Calculates summary statistics.

### JOB C – The Report File
Created `main.py` to load records, generate a summary and save a formatted report with a date-based filename inside the `reports/` directory.

## Technologies Used
- Python
- Regular Expressions (`re`)
- File Handling
- OS Module
- Datetime Module

## Conclusion
This project demonstrates how Python can be used to manage real-world data, identify invalid records and automatically generate structured reports.
