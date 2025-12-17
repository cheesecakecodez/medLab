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

```text
medLab/
├── medlabgo.py      # Main application logic
├── med.py           # Alternate / experimental implementation
├── README.md
├── LICENSE
└── .gitignore
