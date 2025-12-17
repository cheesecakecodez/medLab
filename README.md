# MedLabGo – Medical Lab Test Booking System

MedLabGo is a Python-based command-line application that models a medical laboratory test booking workflow.  
The system recommends diagnostic tests based on patient age, gender, and category, calculates costs, assigns a doctor, and generates/hooks a medical report.

This project was built with a focus on **logical correctness, real-world rule modeling, and end-to-end flow**, rather than UI or presentation.

---

## Problem Statement

Manual medical test booking involves:
- Repetitive data entry
- Error-prone test selection
- Inconsistent billing
- Unstructured patient records

This project attempts to automate that process using rule-based decision logic.

---

## Features

- Rule-based diagnostic test recommendation
- Age-group and gender-driven medical logic
- Automated cost calculation with GST
- Random doctor assignment with contact details
- Patient report generation as a text file
- Date parsing and scheduling logic

---

## Tech Stack

- Language: Python 3
- Libraries:
  - `datetime` for date handling
  - `random` for doctor assignment
- Interface: Command Line
- Data Storage: File-based report generation

---

## Project Structure
medLab/
├── medlabgo.py      # Main application logic
├── med.py           # Alternate / experimental implementation
├── README.md
├── LICENSE
└── .gitignore


 # How It Works

User enters patient details (name, age, gender, address, contact).

System categorizes the patient using age and gender.

Relevant diagnostic tests are suggested.

User selects required tests.
# APPLICATIONS:

Calculates total cost

Applies GST

Assigns a doctor

Generates a medical report

The report is saved locally as:

<PatientName>.txt

# How to Run
## Requirements

Python 3.10 or higher (required for match-case)

Execution
python medlabgo.py

##Output

Printed test list with prices

Final billing amount

Text-based medical report containing:

Patient details

Assigned doctor information

Cost breakdown

Design Notes

Business rules are implemented explicitly rather than abstracted to prioritize clarity.

Input validation is minimal and assumes correct user input.

The system is intentionally CLI-based to focus on logic and flow.

## Limitations

No persistent database

No authentication or authorization

CLI-only interface

Minimal input validation

# Future Scope

Refactor into a Flask REST API

Add frontend (React / Flutter)

Integrate a database (PostgreSQL)

Containerize using Docker

Deploy on a cloud platform

License

This project is licensed under the MIT License.

