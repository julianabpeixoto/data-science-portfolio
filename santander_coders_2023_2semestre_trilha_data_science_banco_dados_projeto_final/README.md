# US School Shootings Analysis

## Project Overview
As the final project of Module 2: Data Base of 'Santander Coders 2023 | 2º Semestre - DS (3)', taught by Aruã de Mello Sousa, this project involves performing exploratory data analysis on the US School Shootings (1970-2022) dataset using Python and PostgreSQL. The goal is to analyze the data, answer specific questions, and gain insights into the patterns and factors related to school shootings in the United States. The analysis revealed several interesting trends and patterns detailed in the file (/adabd_jbp_projeto_final_us_school_shootings.ipynb).

## Objectives

### General Objective
- Conduct an exploratory data analysis of a dataset using Python and PostgreSQL.

### Specific Objectives
1. Load the dataset into PostgreSQL (CHALLENGE).
2. Perform a descriptive analysis of the dataset.
3. Answer the following questions using SQL queries:
   - What is the total number and respective percentage of incidents by state?
   - Which states have the most incidents and the most minor incidents?
   - How many shots were fired per state?
   - How many victims were there per state?
   - Which are the ten states with the highest number of fatal victims?
   - What is the age of the majority of the victims?
   - How many victims per state are between 10 and 22 years old?
   - How many victims were hit by each type of weapon?
   - Of the 2,054 handgun victims, how many were hit in the same incident?
   - In how many incidents was each type of weapon used?
   - In how many incidents was each weapon caliber used?
   - What is the relationship of the shooters to the school?
   - What is the relationship of the victims to the school?
   - How many incidents occurred per year?
   - How many people were victimized annually?
   - Visualize incidents and victims per year.
4. Apply SQL and query knowledge learned during the module.

## About the Dataset
The dataset used is the US School Shootings (1970-2022) available on <a href='https://www.kaggle.com/datasets/shilongzhuang/us-school-shootings-19702022' target='blank'>Kaggle</a>. It is structured as a relational database (compilation of multiple spreadsheets) referenced with a unique incident identification number (incident_id) that links to the following files:

- `incident.csv`
- `weapon.csv`
- `shooter.csv`
- `victim.csv`

This public dataset contains factual and anonymized information about 2,061 school shootings in the United States from 1970 to 2022.

### Tables Description

- **INCIDENT (incident.csv)**: The incident identification number and information about what, where, and when the shooting occurred.
- **VICTIM (victim.csv)**: Contains the incident identification number and details about the victim. Multiple rows will have the same incident identification number if multiple victims exist.
- **SHOOTER (shooter.csv)**: Contains the incident identification number and details about the shooter. Multiple rows with similar incident identification numbers indicate various shooters involved.
- **WEAPON (weapon.csv)**: This file contains the incident identification number and details about the weapon used (including weapons the shooter possessed during the incident but did not fire). Numerous rows would have the same incident identification number if multiple weapons were used.

## Technologies Used

- Python
- PostgreSQL
- Pandas

## Files

- **Data**: Contains the raw dataset files.
  - (/INCIDENT.csv)
  - (/SHOOTER.csv)
  - (/VICTIM.csv)
  - (/WEAPON.csv)
  - 
- **Code**: Contains the Python scripts and SQL queries used for the analysis and the detailed report on the analysis and findings.
  - (/adabd_jbp_projeto_final_us_school_shootings.ipynb)

## Contact

Feel free to contact me with any questions or want to collaborate on future projects.

- **Email**: (jbertolucci@gmail.com)
- **LinkedIn**: (https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: (https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!

---

<p align="center">
  <img src="../../images/neurons_frying_logo.png" alt="Neurons Frying Logo" width="200"/>
</p>
