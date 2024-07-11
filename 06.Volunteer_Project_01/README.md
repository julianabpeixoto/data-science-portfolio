
# Firearms Import Control Cross-Referencing and Matching System

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Motivation](#project-motivation)
3. [Objectives](#objectives)
   - [General Objective](#general-objective)
   - [Specific Objectives](#specific-objectives)
4. [About the Dataset](#about-the-dataset)
5. [Methodology](#methodology)
   - [Import and Initial Processing](#import-and-initial-processing)
   - [Data Cleaning and Preparation](#data-cleaning-and-preparation)
   - [Data Transformation](#data-transformation)
   - [Cross-Referencing and Matching](#cross-referencing-and-matching)
   - [Post-Matching Processing](#post-matching-processing)
   - [Final Data Preparation](#final-data-preparation)
   - [Exporting Results](#exporting-results)
6. [Results and Insights](#results-and-insights)
7. [Challenges and Solutions](#challenges-and-solutions)
8. [Technologies Used](#technologies-used)
9. [Conclusion](#conclusion)
10. [Future Work](#future-work)
11. [Contact](#contact)

## Project Overview
This project aims to create a system for cross-referencing and matching two firearms datasets to identify patterns and connections across documentation and importation data. The goal is to enhance data accuracy and provide meaningful insights into firearm-related import control. It involves extensive data cleaning, transformation, and matching processes to ensure accurate and reliable cross-referencing of firearms data from different sources.

## Project Motivation
As a volunteer supporting data teams in NGOs focused on public safety, I recognized the need for robust data integration and analysis tools. This project leverages data science techniques and collective effort to improve data handling and analysis in firearms import control.

## Objectives

### General Objective
Develop a system to cross-reference and match entries from distinct firearms datasets.

### Specific Objectives
1. Integrate datasets from different sources.
2. Perform data cleaning and preparation.
3. Conduct data transformation.
4. Implement algorithms to match records across datasets.
5. Execute post-matching processing.
6. Explore the matched data to identify patterns and insights.
7. Complete final data preparation.
8. Export results.

## About the Dataset
- **Dataset 1**: Contains information on firearms documentation (12,462 entries and 30 columns).
- **Dataset 2**: Contains details on firearms importation (27,333 entries and 30 columns).

## Methodology

### Import and Initial Processing
- **Documentation Database (df_doc)**: Import an Excel file containing firearms documentation data (12,462 entries and 30 columns), ensuring specific columns are treated as strings to preserve formatting.
- **Importation Database (df_imp)**: Import another Excel file containing firearms importation data (27,333 entries and 30 columns), assigning a default numeric index.

### Data Cleaning and Preparation
- **Column Cleaning**: Standardize column names by converting them to lowercase and replacing non-alphanumeric characters with underscores.
- **Column Renaming**: Simplify and rename specific columns for easier reference.
- **Data Type Enforcement**: Ensure columns have the correct data types (e.g., strings, integers).
- **Missing Values Handling**: Replace NaN values with appropriate defaults (e.g., 'NA' for strings, 0 for integers).
- **Data Harmonization**: Standardize category names across both datasets using predefined mappings.

### Data Transformation
- **Upper/Lower Case Conversion**: Convert specific columns to upper or lower case as needed.
- **Whitespace and Special Character Removal**: Remove spaces, hyphens, and dots from specific columns to ensure consistency.

### Cross-referencing and Matching
- **Subset Creation**: Create subsets of both datasets with relevant columns for matching.
- **Match Level Definition**: Define various match levels (e.g., perfect match, partial match) based on criteria such as serial number, government mark, category, and model.
- **Matching Function**: Implement a function to check match levels between rows of the two datasets.
- **Apply Matching Logic**: Apply the matching function to identify matches and assign match levels.

### Post-Matching Processing
- **Additional Matching**: Perform additional matching for rows that did not find a match in the initial pass.
- **Error Checking**: Implement checks to ensure the accuracy of matches, especially for specific categories and exporting states.

### Final Data Preparation
- **Column Reorganization**: Reorganize columns for clarity and consistency.
- **Merging Data**: Merge the matched documentation and importation datasets to create a final dataset with comprehensive information.

### Exporting Results
- **Export to Excel and CSV**: Export the final matched dataset to both Excel and CSV formats for further analysis or reporting.

## Results and Insights
- Key findings from the analysis, including patterns, correlations, and any significant trends identified.

## Challenges and Solutions
This project was challenging. I encountered several hurdles that required innovative solutions. Following are the three most significant challenges and the solutions to overcome them:

### 1. Data Cleaning and Standardization
- **Challenge**: The datasets come from different sources with varying formats, column names, and data types.
- **Solution**: Standardize column names, enforce consistent data types, handle missing values, harmonize category names, and remove unnecessary characters.

### 2. Accurate Matching of Records
- **Challenge**: Variations in data entries make matching records complex.
- **Solution**: Implement a detailed matching algorithm with multiple criteria to ensure accurate cross-referencing.

### 3. Handling Missing and Incomplete Data
- **Challenge**: Missing or incomplete data can lead to inaccurate analysis.
- **Solution**: Replace missing values with appropriate defaults and perform additional matching for unmatched rows.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: Pandas, Re
- **Tools**: Jupyter Notebook, Git

## Conclusion
This project has successfully developed a robust system for cross-referencing and matching firearms datasets, enhancing data accuracy and providing meaningful insights for firearms import control.

## Future Work
- Explore advanced machine learning techniques for improved record matching.
- Extend the system to include more datasets and broader analysis.
- Collaborate with NGOs to apply the findings in real-world scenarios.

## Contact
Feel free to reach out if you have any questions or want to collaborate on future projects.

- **Email**: jbertolucci@gmail.com
- **LinkedIn**: [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: [JulianaBPeixoto](https://github.com/julianabpeixoto)

---