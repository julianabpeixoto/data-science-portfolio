# Firearms Import Control Cross-Referencing and Matching System

## Table of Contents

1. [Project at a Glance](#project-at-a-glance)
2. [Project Overview](#project-overview)
3. [Project Motivation](#project-motivation)
4. [Objectives](#objectives)
5. [About the Dataset](#about-the-dataset)
6. [Methodology](#methodology)
7. [Main Skills Used](#main-skills-used)
8. [Outputs](#outputs)
9. [Challenges and Solutions](#challenges-and-solutions)
10. [Technologies Used](#technologies-used)
11. [Responsible Data Note](#responsible-data-note)
12. [Conclusion](#conclusion)
13. [Next Steps](#next-steps)
14. [Files](#files)
15. [Contact](#contact)

---

## Project at a Glance

* **Role:** Volunteer data scientist
* **Domain:** Public safety, firearms policy, conflict-affected contexts
* **Main task:** Cross-referencing and matching two heterogeneous datasets
* **Core methods:** Data cleaning, harmonization, record linkage, QA checks, reproducible workflow
* **Tools:** Python, pandas, regular expressions, Jupyter Notebook, Git
* **Data access:** Private source; original data not shared

---

## Project Overview

This project develops a system for cross-referencing and matching two complementary firearms datasets to identify connections across documentation and importation records. The goal is to improve data accuracy and support more reliable analysis of firearm-related import control.

The project involved extensive data cleaning, transformation, harmonization, and matching processes to improve consistency across data from different sources.

---

## Project Motivation

This was a volunteer contribution to a data team supporting an international NGO working on public safety and conflict-affected contexts.

Government and administrative datasets in this domain are often fragmented across systems, with inconsistent formats and partial overlaps. The project responds to a practical need: bringing two separately maintained datasets into a structure that allows them to be analyzed together, with documented assumptions and reproducible code.

---

## Objectives

### General Objective

Develop a system to cross-reference and match entries from two distinct firearms datasets.

### Specific Objectives

1. Integrate datasets from different sources.
2. Perform data cleaning and preparation.
3. Conduct data transformation.
4. Implement logic to match records across datasets.
5. Execute post-matching processing.
6. Explore the matched data to identify patterns.
7. Complete final data preparation.
8. Export results.

---

## About the Dataset

The project worked with two complementary large-scale datasets covering firearms documentation and importation, respectively. Specific volumetric details, field names, and matching criteria are not disclosed in this repository due to the sensitivity of the source data.

---

## Methodology

### Import and Initial Processing

* Import documentation and importation datasets from spreadsheet files.
* Ensure specific columns are treated as strings to preserve formatting.
* Assign appropriate indexes for downstream processing.

### Data Cleaning and Preparation

* Standardize column names by converting them to lowercase and replacing non-alphanumeric characters with underscores.
* Simplify and rename selected columns for easier reference.
* Enforce correct data types across the pipeline.
* Replace missing values with documented defaults where appropriate.
* Harmonize category names across both datasets using predefined mappings.

### Data Transformation

* Apply case normalization to relevant columns.
* Remove whitespace and special characters to improve consistency.
* Prepare selected fields for matching across datasets.

### Cross-Referencing and Matching

* Create subsets of both datasets containing the fields relevant for matching.
* Define a hierarchy of match levels, such as strict and partial matches, based on combinations of identifying fields and contextual attributes.
* Implement a matching function to evaluate match levels between records across the two datasets.
* Apply the matching logic and assign match levels accordingly.

### Post-Matching Processing

* Run additional matching passes for records that did not match in the initial round.
* Apply consistency checks to validate matches and flag inconsistencies for review.

### Final Data Preparation

* Reorganize columns for clarity and consistency.
* Merge the matched documentation and importation datasets into a final consolidated dataset.

### Exporting Results

* Export the final matched dataset to Excel and CSV formats for further analysis and reporting.

---

## Main Skills Used

### Data Analysis

* **pandas:** Used for data manipulation, cleaning, and preprocessing. It enabled efficient handling of large datasets and supported the merging and cross-referencing workflow.

### Data Cleaning and Preparation

* **Regular expressions:** Applied to text manipulation tasks such as standardizing column names, removing special characters, and enforcing consistent data formats.

### Data Transformation

* **String manipulation:** Applied to ensure uniformity in case, remove whitespace, and handle special characters — all critical for accurate matching.

### Matching Logic

* **Custom matching routines:** Designed to apply a hierarchy of match levels across multiple criteria, supporting both strict and partial matches.

### Data Export

* **Excel and CSV handling:** Implemented to make the final matched dataset available in formats suitable for further analysis and reporting.

### Version Control

* **Git:** Used for version control, ensuring systematic tracking of changes and supporting collaboration.

### Reproducible Workflow

* **Jupyter Notebook:** Used to document the analytical workflow, assumptions, processing steps, and outputs in a transparent and reproducible format.

---

## Outputs

The pipeline produced a consolidated dataset that brought together two previously separate sources, allowing the partner NGO’s data team to examine patterns that were difficult to observe when the datasets were considered in isolation.

The work focused on data quality, harmonization, matching logic, and reproducibility rather than inferential modeling. Specific findings derived from the matched data remain confidential to the partner organization.

---

## Challenges and Solutions

The project involved several challenges that required deliberate methodological choices. Three of the most significant are described below.

### 1. Data Cleaning and Standardization

* **Challenge:** The datasets came from different sources, with varying formats, column names, and data types.
* **Solution:** Standardized column names, enforced consistent data types, handled missing values, harmonized category labels, and removed unnecessary characters.

### 2. Accurate Matching of Records

* **Challenge:** Variations in data entries made record matching non-trivial, with risks of both false matches and missed matches.
* **Solution:** Implemented a layered matching approach with multiple criteria, allowing strict and partial matches to be identified separately and reviewed accordingly.

### 3. Handling Missing and Incomplete Data

* **Challenge:** Missing or incomplete fields can lead to inaccurate results if not handled explicitly.
* **Solution:** Replaced missing values with documented defaults and ran additional matching passes for unmatched rows, with assumptions recorded in the notebook.

---

## Technologies Used

* **Programming language:** Python
* **Libraries:** pandas, re
* **Tools:** Jupyter Notebook, Git

---

## Responsible Data Note

This project worked with data from a private source. To respect the confidentiality of the partner organization and the sensitivity of the domain, this repository does not include:

* the original datasets or any extracts of them;
* specific record counts or field names;
* operational matching rules or thresholds used in the pipeline;
* results or findings derived from the matched data.

The repository documents the analytical workflow, methodological choices, data-quality challenges, and reproducibility principles applied during the project.

---

## Conclusion

The project produced a reproducible pipeline to harmonize and match records across two heterogeneous datasets, with documented assumptions and responsible handling of sensitive policy data.

It demonstrates an applied approach to data cleaning, harmonization, record linkage, quality assurance, and reproducible analysis in a public-safety context.

---

## Next Steps

* Explore more advanced record-linkage and probabilistic matching techniques.
* Extend the methodology to additional complementary datasets, where appropriate.
* Continue collaboration with the partner NGO on refinements aligned with their analytical priorities.

---

## Files

* **[Notebook](https://github.com/julianabpeixoto/data-science-portfolio/blob/main/06.Volunteer_Project_01/firearms_datasets_cross_referencing_and_matching_system.ipynb):** Contains a sanitized version of the analytical workflow and implementation structure. Sensitive data, operational rules, thresholds, and partner-specific details are not disclosed.
* **Data:** Data cannot be shared, as it comes from a private source.

---

## Contact

Feel free to reach out with questions or to discuss possible collaborations.

* **Email:** [jbertolucci@gmail.com](mailto:jbertolucci@gmail.com)
* **LinkedIn:** [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
* **GitHub:** [julianabpeixoto](https://github.com/julianabpeixoto)
