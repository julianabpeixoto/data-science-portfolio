# US School Shootings Analysis

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Motivation](#project-motivation)
3. [Objectives](#objectives)
   - [General Objective](#general-objective)
   - [Specific Objectives](#specific-objectives)
4. [About the Dataset](#about-the-dataset)
   - [Tables Description](#tables-description)
5. [Tasks Completed](#tasks-completed)
   - [Data Loading and Initial Inspection](#data-loading-and-initial-inspection)
   - [Descriptive Analysis](#descriptive-analysis)
   - [SQL Query Analysis](#sql-query-analysis)
   - [Visualization](#visualization)
6. [Main Skills and Features Used](#main-skills-and-features-used)
7. [Challenges and Solutions](#challenges-and-solutions)
8. [Results and Insights](#results-and-insights)
9. [Next Steps](#next-steps)
10. [Acknowledgements](#acknowledgements)
11. [Technical Stack](#technical-stack)
12. [Files](#files)
13. [Contact](#contact)

---
## Project Overview
As the final project of Module 3: Database of 'Santander Coders 2023 | 2nd Semester - DS (3)', taught by Aruã de Mello Sousa, this project involves performing exploratory data analysis on the US School Shootings (1970-2022) dataset using Python and PostgreSQL. The goal is to analyze the data, answer specific questions, and gain insights into the patterns and factors related to school shootings in the United States. The analysis revealed several interesting trends and patterns detailed in the [notebook](adabd_jbp_projeto_final_us_school_shootings.ipynb).

## Project Motivation
As a volunteer in two NGOs that work in public safety, I have supported their data teams. This experience inspired me to start working with datasets related to this area. This project is a first step in using data to understand and address the issue of school shootings. In the future, I plan to compare these findings with data from Brazil and the UK to identify common patterns and unique differences.

## Objectives

### General Objective
- Conduct an exploratory data analysis of a dataset using Python and PostgreSQL.

### Specific Objectives
1. Load the dataset into PostgreSQL.
2. Perform a descriptive analysis of the dataset.
3. Formulate and answer the following questions using SQL queries:
   - What is the total number and respective percentage of incidents by state?
   - Which states have the most and the fewest incidents?
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
The dataset used is the US School Shootings (1970-2022) available on [Kaggle](https://www.kaggle.com/datasets/shilongzhuang/us-school-shootings-19702022). It is structured as a relational database (compilation of multiple spreadsheets) referenced with a unique incident identification number (incident_id) that links to the following files:

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

## Tasks Completed

### Data Loading and Initial Inspection
The project began by loading the dataset files into PostgreSQL. This was a challenging but rewarding task that allowed for efficient data querying and management. The data was ingested Using Python's SQLAlchemy and Pandas, and an initial inspection was conducted to understand its structure and content.

### Descriptive Analysis
A thorough descriptive analysis uncovered basic statistics and distributions within the data, including:
- Counting the number of records and unique entries in various columns.
- Identifying and handling missing values.
- Analyze the data types and ensure they are appropriate for the intended analysis.

### SQL Query Analysis
SQL queries were designed and executed to answer specific research questions. This involved:
- Writing complex SQL queries to extract meaningful insights.
- Using aggregate functions to summarize data.
- Applying joins to combine data from different tables.
- Filtering data using WHERE clauses to focus on specific subsets of the dataset.

### Visualization
Various visualizations were created using Python libraries such as Matplotlib and Seaborn to make the findings more accessible and understandable. These visualizations included:
- Bar charts showing the number of incidents per state.
- Line graphs illustrating the trend of incidents over the years.
- Histograms displaying the distribution of victim ages.

## Main Skills and Features Used

- **Libraries**: Pandas, SQLAlchemy, Matplotlib, Seaborn
- **Data Loading and Inspection**:
  - Loading datasets into PostgreSQL using SQLAlchemy
  - Inspecting data types, column names, and missing values
- **SQL Querying**:
  - Writing and executing SQL queries to extract insights
  - Using aggregate functions and joins for comprehensive analysis
- **Exploratory Data Analysis (EDA)**:
  - Statistical summary of numerical columns (mean, median, min, max, standard deviation)
  - Distribution analysis of categorical columns
- **Data Visualization**:
  - Creating visual representations of the data to illustrate findings

## Challenges and Solutions
It was my first time using SQL. In addition to learning the language and integrating it with Python, I needed to install and configure PostgreSQL and pgAdmin4 on my Mac. I referred to documentation and forums on Python and PostgreSQL to resolve these issues.

Initially, I struggled to export DataFrames directly to PostgreSQL tables via Python. After multiple attempts and consultations with documentation, forums, and discussions with ChatGPT, my classmate Anderson Miranda and I discovered that the problem was the version of the SQLAlchemy library I was using (1.4.46). After updating to version 2.0.28, I was able to accomplish this task.

In the notebook, I present two methods used during this process. The first method, more complex and confusing, is demonstrated with the weapon table (which has the fewest columns). The following code creates and deletes the weapon table.

After updating the SQLAlchemy library, the second method was more direct and efficient for inserting all four dataset tables into PostgreSQL.

## Results and Insights
The analysis provided several key insights:
- The states with the highest number of incidents were identified, highlighting regions that may require more attention and resources.
- The analysis of victim ages revealed that a significant number of victims were young, emphasizing the need for targeted interventions.
- Trends over time showed fluctuations in the number of incidents, which could be correlated with policy changes or other external factors.

## Next Steps
Future work could involve a deeper analysis of the factors contributing to school shootings, such as socioeconomic conditions or access to firearms. Additionally, predictive modeling could be applied to forecast future incidents and help in preventive measures.

## Acknowledgements
I want to thank my instructor, Aruã de Mello Sousa, for his guidance throughout this project and the Kaggle community for providing the dataset. I also thank my classmate Anderson Miranda for his valuable assistance.

## Technical Stack
- **Languages**: Python, SQL
- **Database**: PostgreSQL
- **Libraries and Frameworks**: Pandas, SQLAlchemy, Matplotlib, Seaborn
- **Tools**: pgAdmin4, Git

## Files

- **Data**: Contains the raw dataset files.
  - [incident.csv](incident.csv)
  - [shooter.csv](shooter.csv)
  - [victim.csv](victim.csv)
  - [weapon.csv](weapon.csv)
- **Code**: Contains the Python scripts and SQL queries used for the analysis.
  - [Notebook](adabd_jbp_projeto_final_us_school_shootings.ipynb)

## Contact

Feel free to contact me with any questions or to collaborate on future projects.

- **Email**: jbertolucci@gmail.com
- **LinkedIn**: [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: [JulianaBPeixoto](https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!

---
