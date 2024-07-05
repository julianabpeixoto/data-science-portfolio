# Mental Health Treatment Analysis: Enhancing Understanding through Machine Learning

## Table of Contents
1. [Project Overview](#project-overview)
2. [Project Motivation](#project-motivation)
3. [Objectives](#objectives)
   - [General Objective](#general-objective)
   - [Specific Objectives](#specific-objectives)
4. [About the Dataset](#about-the-dataset)
5. [Tasks Completed](#tasks-completed)
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
This is the final project for Module 6: Machine Learning II of 'Santander Coders 2023 | 2nd Semester—DS (3)', taught by Rogério Mainardes. It focuses on developing and evaluating supervised and unsupervised machine learning models for analyzing mental health treatment data, optimizing their hyperparameters, and comparing their performances.

## Project Motivation
Understanding mental health trends is crucial for developing effective public health policies and support programs. This project aims to analyze global mental health trends, identify significant patterns, and test predictive models for mental health treatment.

## Objectives

### General Objective
- Develop and evaluate supervised (SVM or Ensembles) and unsupervised machine learning models to solve a classification problem, optimizing their hyperparameters and comparing their performances based on appropriate evaluation metrics.

### Specific Objectives
1. Select and present the dataset.
2. Conduct exploratory data analysis.
3. Define the target variable and justify its choice.
4. Implement the models.
5. Optimize hyperparameters.
6. Evaluate the models using classification evaluation metrics.
7. Compare and analyze the results.

## About the Dataset
The dataset, obtained from [Kaggle](https://www.kaggle.com/datasets/divaniazzahra/mental-health-dataset), records a global survey on mental health trends, covering variables such as stress, depression, anxiety, subjective well-being, and use of mental health services. The data spans from 2014 to 2015 and includes demographic information like gender, occupation, self-employment status, family history of mental health issues, and more.

## Tasks Completed
1. **Data Loading and Initial Inspection**: Loaded and inspected the dataset for data types, missing values, and distribution.
2. **Descriptive Analysis**: Conducted univariate and bivariate analysis to understand the distribution and relationships between variables.
3. **Data Treatment**: Handled missing values and removed irrelevant columns.
4. **Data Preparation for Supervised Model**: Separated explanatory variables (X) and target (y), encoded categorical variables, balanced classes using SMOTE, and split data into training and test sets.
5. **Supervised Model Implementation**: Implemented XGBoost within a pipeline, evaluated using metrics like accuracy and AUC-ROC, and analyzed variable importance.
6. **Supervised Model Optimization and Adjustment**: Optimized hyperparameters using GridSearchCV, experimented with classification thresholds, and generated evaluation graphs.
7. **Data Preparation for Unsupervised Models**: Encoded categorical variables, normalized data, and separated explanatory variables (X).
8. **K-Means Unsupervised Model**: Applied K-means clustering, evaluated clusters using metrics like Silhouette Coefficient, and visualized clusters.
9. **DBSCAN Unsupervised Model**: Applied DBSCAN, evaluated clusters, and visualized results.

## Main Skills and Tools Used
- **Programming Languages**: Python
- **Libraries**: Pandas, NumPy, NLTK, SpaCy, Scikit-learn, Matplotlib, Seaborn
- **Techniques**: Data cleaning and preprocessing, exploratory data analysis (EDA), model implementation and evaluation, hyperparameter tuning, data visualization

## Challenges and Solutions
- **Imbalanced Classes**: Addressed using SMOTE for balanced class distribution.
- **Text Data Preprocessing**: Implemented thorough text cleaning and preprocessing steps.
- **Hyperparameter Tuning**: Utilized GridSearchCV with StratifiedKFold for optimal hyperparameter selection.

## Results and Insights
The analysis revealed significant insights into the factors affecting mental health treatment. The XGBoost model, after hyperparameter tuning, achieved the highest accuracy and AUC-ROC scores, indicating its robustness in predicting mental health treatment. Key variables influencing predictions included
self-employment status,
family history of mental health issues, and
changes in habits or sleep patterns.

## Next Steps
- As suggested by the instructor, select variables more specifically for the K-means model, even before applying dimensionality reduction. This ensures that the variables adding the most value and having the strongest associations with the final values are included.
- Explore advanced machine learning techniques such as ensemble or deep learning models to improve prediction accuracy. 
- Additionally, studying the impact of different demographic variables on mental health treatment can provide deeper insights and help tailor interventions more effectively. It is also recommended that specific techniques for handling multi-class problems in mental health datasets be investigated. 

## Acknowledgements
Thanks to the instructor and the data community for their support and resources.

## Technical Stack
- **Languages**: Python
- **Libraries and Frameworks**: Pandas, NumPy, NLTK, SpaCy, Scikit-learn, Matplotlib, Seaborn
- **Tools**: Jupyter Notebook, Git

## Files
- **Notebook**: Contains the full analysis and model implementation.
  - [Notebook](https://github.com/julianabpeixoto/neurons-frying/blob/main/05.SC2023_Module6/jbp_projeto_final_ada_ml_II.ipynb)
- **Data**: Contains the dataset used for the project.
  - [Data Source](https://www.kaggle.com/datasets](https://www.kaggle.com/datasets/divaniazzahra/mental-health-dataset)

## Contact

Feel free to contact me with any questions or to collaborate on future projects.

- **Email**: jbertolucci@gmail.com
- **LinkedIn**: [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub**: [JulianaBPeixoto](https://github.com/julianabpeixoto)

Thank you for visiting my portfolio!
