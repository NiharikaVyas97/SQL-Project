# Hospital Management Database Project

## Project Overview

This project involves creating a **Hospital Management Database** using **MS SQL Server**. The database manages essential information about patients, doctors, appointments, treatments, and medical records in a hospital setting. This project includes multiple SQL queries ranging from basic to advanced levels using various SQL functions and window functions such as `ROW_NUMBER()`, `RANK()`, and `LAG()`.

## Features

- Manage **patients**, **doctors**, **appointments**, **treatments**, and **medical records**.
- Track patient appointments, treatment history, and doctor specializations.
- Use advanced SQL queries to retrieve valuable insights such as:
  - Total treatments per doctor.
  - Highest treatment costs.
  - Latest appointments per patient.
  - Running total of treatment costs.
  - Difference in treatment costs for each patient.
  
## Database Structure

The database consists of five main tables:

1. **Patients**: Stores information about patients such as names, DOB, contact details, and gender.
2. **Doctors**: Stores information about doctors including specialization, contact information, and hire date.
3. **Appointments**: Tracks patient appointments with doctors.
4. **Treatments**: Contains treatment details including treatment type, start and end dates, cost, and associated doctor.
5. **MedicalRecords**: Contains diagnosis, prescription, and medical notes related to patient treatments.

## Advanced Features
This project demonstrates the following advanced SQL concepts:

1. Window Functions: Usage of ROW_NUMBER(), LAG(), RANK() to provide complex analysis over partitions of data.
2. Aggregate Functions: Operations like SUM(), COUNT(), and AVG() for summarizing data.
3. Joins and Subqueries: Retrieving data from multiple tables using joins and applying subqueries for conditional queries.
4. Data Filtering: Using HAVING and GROUP BY to filter and organize the dataset.

### ER Diagram

```text
Patients <-- Appointments --> Doctors
Patients <-- Treatments --> Doctors
Treatments <-- MedicalRecords --> Patients

