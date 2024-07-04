# Predicting Firearm Brands: A Machine Learning Approach to Enhance Police Intelligence and Cataloging

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
This project is the final project for Module 5: Machine Learning I of 'Santander Coders 2023 | 2nd Semester—DS (3)', taught by Thiago Tavares Magalhães. It applies machine learning techniques to analyze a dataset of firearm seizures. Using Python and relevant libraries, the goal is to develop a machine-learning model to classify unidentified firearm brands in a dataset where brands are labeled as 'Not Identified.' The model could assist in more efficient research and cataloging processes. This project marks the first time I learned and created a machine-learning model, making it a significant milestone in my data science journey.

## Project Motivation
Accurately identifying firearm brands is crucial for police work for two main reasons:
1. Without correct brand identification, intelligence reports lose value as they cannot determine the manufacturer's nationality and potential entry routes into the country.
2. Inaccurate brand identification hampers national tracking and renders international requests for tracing impossible without complete firearm data (type, brand, model, caliber, and serial number).

## Objectives

### General Objective
- Apply machine learning techniques to analyze and predict firearm brands in the provided dataset.

### Specific Objectives
1. Load and preprocess the dataset.
2. Perform exploratory data analysis (EDA).
3. Implement and evaluate different machine learning models.
4. Optimize hyperparameters and apply the final model to predict unidentified brands.

## About the Dataset
The dataset includes information on firearm and ammunition seizures by the Military and Civil Police in Rio de Janeiro from 2015 to 2017. The data was obtained via the LAI (Lei de Acesso à Informação) from the Instituto de Segurança Pública do Rio de Janeiro (ISP).

### Data Structure
- The dataset consists of three .xlsx files, each representing a year from 2015 to 2017, detailing the firearm seizures.
- The analysis focuses on firearms-related columns, excluding irrelevant data for the classification task.

## Tasks Completed

### Data Loading and Initial Inspection
- Imported data from the 2015, 2016, and 2017 firearm seizure records.
- Checked data types, missing values, and distribution.

### Descriptive Analysis
- Analyzed distributions of categorical and numerical variables.
- Visualized data to understand feature characteristics and relationships better.

### Visualization
- Created visualizations using Matplotlib and Seaborn to illustrate data insights and model performance.

## Main Skills and Tools Used
- **Programming Languages**: Python
- **Libraries**:
  - **Pandas**: Data manipulation and analysis
  - **NumPy**: Numerical computations
  - **Matplotlib** and **Seaborn**: Data visualization
  - **Scikit-learn**: Machine learning algorithms and model evaluation
- **Techniques**:
  - Data cleaning and preprocessing
  - Exploratory data analysis (EDA)
  - Model implementation and evaluation
  - Hyperparameter tuning
  - Data visualization

## Challenges and Solutions

### Serial Number (sn) Variable

#### Description
A firearm's serial number (sn) is a unique numeric or alphanumeric code assigned to each gun produced by licensed manufacturers. It serves as a unique identifier distinguishing a specific firearm from others. 

### Functions
1. **Tracking and Record-Keeping**: Allows authorities to trace the origin and history of a firearm from manufacturing through distribution to its current owner.
2. **Crime Prevention and Resolution**: SNs help verify whether a firearm was stolen or used in criminal activities, aiding law enforcement in crime prevention and resolution.
3. **Legal Compliance**: SNs are required in many countries and international treaties. Manufacturers and importers must inscribe these numbers clearly and indelibly on firearms for control and safety.
4. **Quality Control**: Manufacturers use SNs to control production quality and identify specific batches of firearms, facilitating the recall or repair of defective models.

### Problems Encountered
- Each manufacturer, even within the same country (e.g., Brazil), follows specific patterns that may change over the years. Some manufacturers allow identical serial numbers for different models or calibers within their production.
- The serial number marking can wear out over time, be tampered with, or be removed to hinder police work and increase impunity for those diverting or purchasing diverted firearms.

### Solution
In this dataset, the serial number (sn) is filled out in many different ways, requiring multiple checks and cleaning to address these values adequately. To solve this inconsistency in the data, I conducted a detailed data-cleaning process:
1. **Identifying Unwanted Values**: I identified and marked records with problematic serial numbers, such as duplicates or inconsistencies.
2. **Standardizing Formats**: Normalized serial number formats where possible to ensure consistency across records.
3. **Handling Missing and Altered Values**: Addressed missing or altered serial numbers by using placeholder values or excluding these records from critical analyses.
4. **Verification and Validation**: Implemented checks to ensure cleaned serial numbers aligned with known manufacturer patterns and legal standards.

### Special Techniques Used
- Opted for **BinaryEncoder** to transform categorical and numerical variables due to its efficiency in handling many categories. BinaryEncoder transforms a categorical variable into log2(n) new columns, where n is the number of unique categories. This reduces the dataset's dimensionality while maintaining significant information. I tested OneHot encoding, but the results were not satisfactory.
- Used **StratifiedKFold** for cross-validation to ensure each training and test set has the same proportion of examples in each class as the entire dataset. This helped address category imbalance, which would have been problematic for the model if not handled. The configuration *shuffle=True* and *random_state=42* ensured consistent shuffling before splitting into folds, preventing sample selection biases and allowing result reproducibility.

## Results and Insights
The analysis and models provided valuable insights into the distribution and characteristics of firearm brands. After hyperparameter tuning, the Random Forest model achieved the highest accuracy and was used for final predictions. The RandomForest model proved to be more effective for this application:
- Besides providing higher overall accuracy than KNN, it showed a better balance between precision and recall (higher F1-scores) and consistently good performance in majority classes. 
- For the TAURUS brand, for example, with the highest number of samples, RF had an F1-score of 0.94, while KNN had 0.93. 
- For brands like BUL and GIRSAN, with fewer samples, RF achieved scores of 1.00, demonstrating its effectiveness in less frequent categories. This aspect is particularly relevant given the imbalanced dataset.

The consulted expert revealed that in cases where it is possible to identify the brand by a pattern in the serial number crossed with the caliber (e.g., .38 revolvers), representing 56 of the 66 analyzed weapons, the model accurately predicted 100% of the brands.

## Next Steps
Future work could explore advanced machine learning techniques, such as ensemble and deep learning, and apply the models to a broader dataset to enhance predictive accuracy. Additionally, it is recommended to delve deeper into problems involving many classes. Although I lack personal experience in this area, I suspect there are specific techniques to handle such challenges, especially when grouping different classes to reduce the number of possible outputs from the model is not feasible.

## Acknowledgements
Thanks to Thiago Tavares Magalhães for helping me during the module and the project, the specialist on firearms, and the data community for their support and resources.

## Technical Stack
- **Languages**: Python
- **Libraries and Frameworks**: Pandas, Matplotlib, Seaborn, Scikit-learn, TensorFlow/Keras
- **Tools**: Jupyter Notebook, Git

## Files
- **Notebook**: Contains the full analysis and model implementation.
  - [Notebook](https://github.com/julianabpeixoto/neurons-frying/blob/main/04.SC2023_Module5/JulianaBertolucciPeixoto_jbp_projeto_final_ada_MachineLearningI.ipynb)
- **Data**: Contains the dataset used for the project.
  - [Data Source](https://www.isp.rj.gov.br)

## Contact

Feel free to contact me with any questions or to collaborate on future projects.

- **Email**: jbertolucci@gmail.com
- **LinkedIn**: [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: [JulianaBPeixoto](https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!

---
