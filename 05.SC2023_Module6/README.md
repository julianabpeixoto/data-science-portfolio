# Mental Health Treatment Analysis — Machine Learning on Survey Data

**Mental health · Public health analytics · Classification · Survey data · Responsible ML**

## Table of Contents

1. [Project at a Glance](#project-at-a-glance)
2. [Project Overview](#project-overview)
3. [Project Context](#project-context)
4. [Research Question](#research-question)
5. [Objectives](#objectives)
6. [About the Dataset](#about-the-dataset)
7. [Methodology](#methodology)
8. [Models and Evaluation](#models-and-evaluation)
9. [Key Findings](#key-findings)
10. [Limitations](#limitations)
11. [Responsible Data and Interpretation](#responsible-data-and-interpretation)
12. [Main Skills and Tools Used](#main-skills-and-tools-used)
13. [Next Steps](#next-steps)
14. [Acknowledgements](#acknowledgements)
15. [Files](#files)
16. [Contact](#contact)

---

## Project at a Glance

* **Role:** Data science student project / applied machine learning analysis
* **Domain:** Mental health, public health analytics, survey data
* **Main task:** Explore factors associated with reported mental health treatment-seeking behavior
* **Target variable:** Whether respondents reported seeking mental health treatment
* **Core methods:** Exploratory data analysis, preprocessing, supervised classification, hyperparameter tuning, unsupervised clustering, model evaluation
* **Tools:** Python, pandas, NumPy, scikit-learn, XGBoost, matplotlib, seaborn, Jupyter Notebook
* **Data source:** Public Kaggle dataset

---

## Project Overview

This project explores a mental health survey dataset to identify factors associated with whether respondents reported seeking mental health treatment.

It applies exploratory data analysis, supervised classification models, hyperparameter tuning, and unsupervised clustering methods to compare model behavior and reflect on the responsible use of machine learning in mental health-related data.

The project was developed as the final assignment for **Module 6: Machine Learning II** of **Santander Coders 2023 | Data Science**, taught by **Rogério Mainardes**.

---

## Project Context

Mental health data requires careful analysis and responsible interpretation. Predictive models can help explore patterns in survey data, but they should not be interpreted as diagnostic tools, clinical screening instruments, or substitutes for professional judgment.

This project uses machine learning as an exploratory tool to examine patterns associated with treatment-seeking behavior in a mental health survey dataset.

---

## Research Question

Which demographic, occupational, and self-reported mental health-related variables are associated with whether respondents reported seeking mental health treatment?

---

## Objectives

### General Objective

Develop and evaluate supervised and unsupervised machine learning models to explore a classification problem related to mental health treatment-seeking behavior.

### Specific Objectives

1. Select and present the dataset.
2. Conduct exploratory data analysis.
3. Define and justify the target variable.
4. Prepare the data for supervised and unsupervised models.
5. Implement classification models.
6. Optimize hyperparameters.
7. Evaluate models using appropriate classification metrics.
8. Compare and interpret model performance.
9. Explore unsupervised clustering methods.
10. Reflect on limitations and responsible interpretation.

---

## About the Dataset

The dataset was obtained from Kaggle and contains self-reported survey responses related to mental health, work context, demographic characteristics, and use of mental health services.

Variables include information such as gender, occupation, self-employment status, family history of mental health issues, reported changes in habits, and whether respondents sought mental health treatment.

Because the dataset is based on self-reported survey responses, results should be interpreted as exploratory and dataset-specific.

[Data Source](https://www.kaggle.com/datasets/divaniazzahra/mental-health-dataset)

---

## Methodology

### Data Loading and Initial Inspection

* Loaded the dataset and inspected its structure.
* Reviewed data types, missing values, and variable distributions.
* Identified columns requiring cleaning, encoding, or exclusion.

### Exploratory Data Analysis

* Conducted univariate and bivariate analysis.
* Explored the distribution of the target variable.
* Examined relationships between treatment-seeking behavior and selected demographic, occupational, and mental health-related variables.

### Data Treatment

* Handled missing values.
* Removed irrelevant or low-value columns.
* Standardized categorical variables where needed.
* Prepared the dataset for supervised and unsupervised modeling.

### Supervised Learning Preparation

* Defined the target variable.
* Separated explanatory variables and target variable.
* Encoded categorical variables.
* Split the data into training and test sets.
* Tested SMOTE for class imbalance, but kept the BinaryEncoder in the final model, as SMOTE did not change the results.

### Unsupervised Learning Preparation

* Encoded categorical variables.
* Normalized selected variables.
* Prepared explanatory variables for clustering analysis.

---

## Models and Evaluation

### Supervised Models

The project tested supervised classification models, with emphasis on tree-based ensemble methods.

The main supervised model was:

* **XGBoost classifier**

Model evaluation included:

* accuracy;
* AUC-ROC;
* confusion matrix;
* classification metrics;
* threshold adjustment;
* feature-importance analysis.

Hyperparameter optimization was conducted using:

* **GridSearchCV**

### Unsupervised Models

The project also explored clustering methods to identify possible groupings in the dataset.

Models included:

* **K-Means**
* **DBSCAN**

Evaluation and interpretation included:

* cluster visualization;
* comparison of clustering outputs;
* Silhouette Coefficient, where appropriate.

---

## Key Findings

The tuned XGBoost model reached an accuracy of approximately 0.78 and an AUC-ROC of approximately 0.87 on the test set, performing marginally better than the untuned baseline configuration — the difference between the two was small.

Feature-importance analysis pointed to self-reported behavioral and mental-health variables as the most influential: mood swings, mental health history, changes in habits, and growing stress ranked highest, followed by days indoors and family history.

The unsupervised methods did not produce well-defined clusters: K-Means returned low silhouette scores (around 0.02 and below) and high Davies-Bouldin indices, and DBSCAN classified most points as noise — the dataset does not separate into clear groups under these methods.

These findings are exploratory and dataset-specific. They do not establish causality and should not be used as clinical recommendations.

---

## Limitations

This project has important limitations:

* The dataset is based on self-reported survey responses.
* The data may not be representative of broader populations.
* The models identify statistical patterns in the available data but do not establish causal relationships.
* Model performance may be affected by class imbalance, survey design, missing values, and variable encoding choices.
* Mental health is a sensitive domain, and predictive outputs require careful interpretation.
* The project should not be used for diagnosis, individual-level decision-making, or clinical screening without further validation and ethical review.

---

## Responsible Data and Interpretation

Because this project deals with mental health-related data, the analysis was approached with caution.

Key principles considered:

* avoid interpreting predictions as diagnoses;
* avoid treating model outputs as clinical recommendations;
* distinguish association from causality;
* recognize possible bias in self-reported survey data;
* interpret feature importance carefully;
* communicate findings as exploratory and dataset-specific;
* consider the ethical implications of applying machine learning to mental health data.

---

## Main Skills and Tools Used

### Programming and Data Analysis

* **Python**
* **pandas**
* **NumPy**

### Machine Learning

* **scikit-learn**
* **XGBoost**
* **SMOTE**
* **GridSearchCV**

### Data Visualization

* **matplotlib**
* **seaborn**

### Analytical Techniques

* Data cleaning and preprocessing
* Exploratory data analysis
* Classification modeling
* Hyperparameter tuning
* Model evaluation
* Feature-importance interpretation
* Clustering analysis

### Tools

* Jupyter Notebook
* Git / GitHub

---

## Next Steps

Potential future improvements include:

* refining variable selection before applying clustering methods;
* comparing additional supervised models using consistent validation procedures;
* exploring explainability methods, such as SHAP, to improve interpretation of model behavior;
* testing model stability across different train-test splits;
* further examining the role of demographic and occupational variables in treatment-seeking behavior;
* improving documentation of preprocessing decisions and model assumptions.

---

## Acknowledgements

This project was developed as part of **Santander Coders 2023 | Data Science**, in the **Machine Learning II** module taught by **Rogério Mainardes**.

---

## Files

* **[Notebook](./jbp_projeto_final_ada_ml_II.ipynb):** Contains the full exploratory analysis, preprocessing, model implementation, evaluation, and visualizations.
* **[Data Source](https://www.kaggle.com/datasets/divaniazzahra/mental-health-dataset):** Public Kaggle dataset used in the project.

---

## Contact

Feel free to reach out with questions or to discuss possible collaborations.

* **Email:** [jbertolucci@gmail.com](mailto:jbertolucci@gmail.com)
* **LinkedIn:** [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
* **GitHub:** [julianabpeixoto](https://github.com/julianabpeixoto)
