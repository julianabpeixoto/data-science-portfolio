# Statistical Analysis of School Shootings in the U.S. concerning City Population

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Motivation](#project-motivation)
3. [Objectives](#objectives)
   - [General Objective](#general-objective)
   - [Specific Objectives](#specific-objectives)
4. [About the Dataset](#about-the-dataset)
5. [Tasks Completed](#tasks-completed)
   - [Data Loading and Initial Inspection](#data-loading-and-initial-inspection)
   - [Descriptive Analysis](#descriptive-analysis)
   - [Hypothesis Testing Analysis](#hypothesis-testing-analysis)
   - [Visualization](#visualization)
6. [Main Skills and Tools Used](#main-skills-and-tools-used)
7. [Challenges and Solutions](#challenges-and-solutions)
8. [Results and Insights](#results-and-insights)
9. [Next Steps](#next-steps)
10. [Acknowledgements](#acknowledgements)
11. [Technical Stack](#technical-stack)
12. [Files](#files)
13. [Contact](#contact)

---

## Project Overview
As the final project of Module 4: Statistics of 'Santander Coders 2023 | 2nd Semester - DS (3)', taught by Lucas Hermeto, this project analyzes the frequency of school shootings in the US relative to city population sizes from 1970 to 2022. I chose to continue with the analysis initiated in the [previous module](https://github.com/julianabpeixoto/neurons-frying/blob/main/santander_coders_2023_2semestre_trilha_data_science_banco_dados_projeto_final/README.md#main-skills-and-features-used) to deepen my learning and analysis. By using Python and data visualization libraries, the goal is to uncover patterns that can inform public policies and preventive measures.

## Project Motivation
School shootings have been a persistent and tragic issue in the United States, impacting countless lives and raising urgent questions about safety, gun control, and community well-being. This project aims to understand the patterns and underlying factors associated with school shootings from 1970 to 2022. Analyzing these incidents about city populations and legislative changes aims to provide data-driven insights that can inform policymakers, educators, and community leaders in their efforts to prevent future tragedies and create safer environments for students.

## Objectives

### General Objective
Perform an exploratory data analysis of two datasets to test 3 hypotheses:
- In the United States, the majority of school shootings that occurred between 1970 and 2022 with the use of firearms happened in cities with a total population 20% smaller than the median population of US cities in 2022.
- Lower levels of gun legislation (2023) are related to higher numbers of school shootings with firearms (1970-2022).
- The passage of time (measured in decades) and the level of gun legislation (2023) have a statistically significant effect on the total number of school shootings with firearms (1970-2020).

### Specific Objectives
1. Load and inspect the dataset.
2. Perform a descriptive analysis of the data.
3. Formulate and test statistical hypotheses.
4. Visualize the results clearly and informatively.

## About the Dataset
To test the hypotheses, two datasets were used and are described below:
- **US School Shootings (1970-2022)**: Available on Kaggle, this dataset contains factual and anonymized information about 2,061 school shootings in the United States that occurred between 1970 and 2022. The data is structured as a relational database, with multiple tables linked by a unique incident identification number (incident_id). The tables include details about the incidents, victims, shooters, and weapons used.
- **US Census Bureau, 2022 American Community Survey 1-Year Estimates**: Available on the United States Census Bureau website, this dataset consists of one table that provides observations on the estimated population of all US cities. The data is based on a sample and includes a margin of error representing the uncertainty of the estimates. The 90% margin of error indicates the range within which the true population value likely falls. Estimates are also subject to non-sampling errors.

## Tasks Completed

### Data Loading and Initial Inspection
The data was loaded and inspected to understand its structure and content. This comprehensive process included checking data types, identifying missing values, and gaining an initial understanding of the data distribution.

### Descriptive Analysis
A descriptive analysis was performed to obtain basic statistics and distributions of the data. This included:
- Counting the number of records and unique entries in various columns.
- Identifying and handling missing values.
- Analyze data types and ensure they are appropriate for the intended analysis.

### Hypothesis Testing Analysis
Hypotheses were formulated and tested to answer specific questions about the distribution of cities in relation to the average total population.

### Visualization
Various visualizations were created using Python libraries such as Matplotlib and Seaborn to make the findings more accessible and understandable. These visualizations included:
- Bar charts showing the percentage distribution of cities.
- Pie charts to visualize the composition of categories.
- Area charts to show trends over time.
- Density plots to visualize the distribution of population data.

![Area Chart](image-1.png)
*Figure 1: Distribution of Incidents Over Decades by State*

![Bar Plot](image-2.png)
*Figure 2: Number of Shootings by Decade and Level of Gun Legislation*


## Main Skills and Tools Used

- **Libraries**: Pandas, Matplotlib, Seaborn
- **Data Loading and Inspection**:
  - Loading datasets using Pandas
  - Inspecting data types, column names, and missing values
- **Statistical Analysis**:
  - Conducting hypothesis tests
  - Using statistical functions to summarize data
- **Data Visualization**:
  - Creating visual representations of the data to illustrate findings

## Challenges and Solutions
One of the main challenges was effectively manipulating and visualizing the data. By consulting documentation and forums, overcoming these challenges and creating clear and informative visualizations was possible.

## Results and Insights
The analysis uncovered several significant insights about the distribution of cities in relation to the average total population. For instance, it revealed that many cities have a population below the average, which could have profound implications for resource allocation and public policies.

## Next Steps
Future work could involve a deeper analysis of the factors contributing to the population distribution of cities, such as socioeconomic conditions and public policies. Additionally, predictive models could be applied to forecast future trends.

## Acknowledgements
I want to thank my instructor for the insights and feedback and the data community for their valuable support and resources.

## Files

- **Data**: Contains the raw dataset files.
  - [US School Shootings (1970-2022)](INCIDENT.csv)
  - [US Census Bureau, 2022 American Community Survey 1-Year Estimates](ACSDT1Y2022.B01003-Data.csv)
- **Code**: Contains the Python scripts and notebooks used for the analysis.
  - [Notebook](jbp_projeto_final_ada_estatistica_I.ipynb)

## Contact

Feel free to contact me with any questions or to collaborate on future projects.

- **Email**: jbertolucci@gmail.com
- **LinkedIn**: [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: [JulianaBPeixoto](https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!

---
