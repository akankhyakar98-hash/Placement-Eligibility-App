#  Placement Eligibility Streamlit Application
This is an interactive Streamlit application engineered to transform raw student data into actionable placement intelligence. It provides a comprehensive, data-driven framework for assessing candidate suitability across key domains: technical mastery, essential soft skills, and placement readiness metrics
## Project Overview

This project allows users (like placement teams or college admins) to:

Filter students based on custom eligibility criteria  
Analyze batch-wise performance and placement trends  
Generate real-time reports with interactive visualizations  
Export filtered results to CSV

---

## Tech Stack

- Python (OOP structure)
- Streamlit (frontend + UI)
- MySQL (relational database)
- Faker (synthetic data generation)
- Pandas (data manipulation)

---

## Prerequisites

-1. Python: Ensure you have Python 3.8+ installed.

-2. Dependencies: we will need the following Python packages: streamlit, pandas, sqlite3, and Faker (for generating synthetic data in main.py).

## Data Foundation Setup (main.py)
The main.py script automatically synthesizes 500 detailed student records and provisions the SQLite database (placement_eligibility.db). This database is structured with four linked tables: Students, Programming, SoftSkills, and Placements.
- Output:  This process creates the persistent placement_data.db file in your project directory.
## Launch the Dashboard (app.py)
With the data foundation secured, initiate the interactive dashboard: 
Run the following command in your terminal: streamlit run app.py . The application will launch automatically in your default web browser.
## Dashboard Capabilities
The application is divided into two distinct, powerful analysis modules accessible via the sidebar:

-1. Candidate Filtering Engine:This module serves as a predictive model, allowing users to define strict minimum thresholds for candidate eligibility. Inputs are configured using intuitive dropdown menus (select boxes) for criteria such as:
Technical Mastery: Minimum problems solved, project scores, and certification requirements.

Essential Soft Skills: Base scores for communication, teamwork, presentation, critical thinking, and more.
Placement Metrics: Required mock interview performance and internship experience.

-2. Strategic Data Insights:This module provides instant access to crucial analytical reports, offering a strategic overview of cohort performance. Key performance indicators and analysis points include:
Comparative analysis of technical scores across different student batches.

Identification of top placement-ready students based on composite scoring.

Visual distribution of Mock Interview Scores, categorized into performance tiers (e.g., 'Poor', 'Good', 'Excellent').


- Users can select any query to view the underlying SQL logic, the resultant data table, and an automatically generated visual chart for quick interpretation.






