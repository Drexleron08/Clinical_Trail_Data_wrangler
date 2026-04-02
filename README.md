# Clinical_Trail_Data_wrangler
Clinical Trial Data Wrangler: Automated Patient Screening Pipeline

📌 Project Overview
In clinical research, data is often siloed across different departments—demographics from administration, lab results from the pathology wing, and dosage logs from the pharmacy.This project simulates a Phase II Clinical Trial environment. It uses Python and the Pandas library to extract, clean, and merge disparate datasets into a single "Analysis-Ready" cohort. The pipeline automates the identification of patients who meet specific clinical inclusion/exclusion criteria, reducing manual error in trial recruitment.

🎯 Key ObjectivesData Integration: 
Perform complex relational joins (inner and left merges) to link patient demographics with longitudinal lab results and treatment logs.
Clinical Validation: Implement automated filtering logic based on medical protocols (e.g., Age $\ge 18$, Systolic BP $\le 140$ mmHg).
Data Quality Assurance: Handle missing clinical values (NaNs) using statistically sound imputation methods (Mean/Median) while maintaining study integrity.
Feature Engineering: Use custom Python functions and .apply() to categorize raw continuous data (e.g., converting Glucose mg/dL into "Normal", "Prediabetic", or "Diabetic" classifications).

🛠️ Tech Stack & Skills
Language: Python 3.14Primary
Library: Pandas (Advanced Data Manipulation)
Visualization: Seaborn & Matplotlib (Efficacy and Demographic Reporting)
Concepts: Relational Algebra, Data Imputation, Clinical Informatics, Vectorized Operations.

📂 Dataset Structure
The project utilizes three simulated "messy" CSV files to mimic real-world Electronic Health Records (EHR):
demographics.csv: Contains Patient ID, Age, Sex, and Baseline Blood Pressure.
lab_results.csv: Records Cholesterol and Glucose levels across different visit dates.
dosage_logs.csv: Tracks the specific treatment arm (Drug A vs. Placebo) and dosage levels.

📊 Methodology & Results
ETL Process: Data was ingested and cleaned of "Chained Assignment" errors to ensure compatibility with modern Pandas Copy-on-Write (CoW) standards.
Filtering: Out of the initial population, approximately 41% of patients were excluded for not meeting the age or baseline health requirements.
Efficacy Analysis: Preliminary visualizations (Boxplots) indicate a statistically visible difference in glucose regulation between the treatment and placebo groups.

🩺 About the Author
As a student pursuing Data Science, I developed this project to bridge the gap between clinical medicine and data engineering. My goal is to leverage computational tools to accelerate medical research and improve patient outcomes through data-driven insights.
