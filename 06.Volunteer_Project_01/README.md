# Firearms Import Control Cross-Referencing and Matching System

**Public safety · Firearms policy · Data quality · Record linkage · Responsible data**

## Table of Contents

1. [Project at a Glance](#project-at-a-glance)
2. [Note on the Public Notebook](#note-on-the-public-notebook)
3. [Project Overview](#project-overview)
4. [Project Motivation](#project-motivation)
5. [Objectives](#objectives)
6. [About the Dataset](#about-the-dataset)
7. [Methodology](#methodology)
8. [Main Skills Used](#main-skills-used)
9. [Outputs](#outputs)
10. [Challenges and Solutions](#challenges-and-solutions)
11. [Technologies Used](#technologies-used)
12. [Responsible Data Note](#responsible-data-note)
13. [Conclusion](#conclusion)
14. [Next Steps](#next-steps)
15. [Files](#files)
16. [Contact](#contact)

---

## Project at a Glance

- **Role:** Volunteer data scientist
- **Domain:** Public safety, firearms policy, conflict-affected contexts
- **Main task:** Cross-referencing and matching two heterogeneous datasets
- **Core methods:** Data cleaning, harmonization, record linkage, QA checks, reproducible workflow
- **Tools:** Python, pandas, regular expressions, Jupyter Notebook, Git
- **Data access:** Private source; original data not shared
- **Repository version:** Sanitized methodological version for portfolio use

---

## Note on the Public Notebook

The notebook available in this repository is a **sanitized version prepared for portfolio purposes**.

It uses synthetic or abstracted examples and does **not** reproduce the original datasets, operational matching rules, thresholds, record identifiers, field names, source-specific labels, partner-specific validation criteria, or findings from the partner organization.

Its purpose is to demonstrate the analytical structure, data-cleaning workflow, record-linkage approach, documentation practices, and responsible handling of sensitive data.

This means the public notebook should not be interpreted as the full operational pipeline used in the original project. It is a methodological demonstration designed to protect confidential information while still showing the technical and analytical approach.

---

## Project Overview

This project documents the development of a system for cross-referencing and matching two complementary firearms-related datasets to identify connections across documentation and importation records.

The goal was to improve data quality and support more reliable analysis of firearm-related import control in a sensitive public-safety context.

The project involved extensive data cleaning, transformation, harmonization, and matching processes to improve consistency across data from different sources. The public version of this repository focuses on the analytical workflow and methodological structure, while protecting sensitive data, operational rules, and partner-specific information.

---

## Project Motivation

This was a volunteer contribution to a data team supporting an international NGO working on public safety and conflict-affected contexts.

Government and administrative datasets in this domain are often fragmented across systems, with inconsistent formats, partial overlaps, missing information, and different data-entry conventions. These issues can make it difficult to analyze related records together and to produce reliable evidence for policy and research.

The project responded to a practical need: bringing two separately maintained datasets into a structure that allowed them to be compared, harmonized, and analyzed together, with documented assumptions and reproducible code.

---

## Objectives

### General Objective

Develop a reproducible system to cross-reference and match entries from two distinct firearms-related datasets.

### Specific Objectives

1. Integrate datasets from different sources.
2. Perform data cleaning and preparation.
3. Standardize column names, formats, and selected variables.
4. Apply documented missing-value handling strategies.
5. Harmonize category names across datasets.
6. Prepare selected fields for cross-referencing.
7. Implement a structured matching workflow.
8. Classify results into broad match categories for review.
9. Apply consistency checks and quality-assurance flags.
10. Prepare a consolidated dataset for further analysis and reporting.
11. Document the workflow while protecting sensitive data and operational details.

---

## About the Dataset

The project used two complementary large-scale datasets covering firearms-related documentation and importation records, respectively.

Specific volumetric details, field names, record identifiers, matching criteria, thresholds, and operational rules are not disclosed in this repository due to the sensitivity of the source data and the confidentiality of the partner organization.

The public notebook uses sanitized, synthetic, or abstracted examples to demonstrate the methodological structure without exposing the original data.

---

## Methodology

### 1. Import and Initial Processing

- Import documentation and importation datasets from spreadsheet files.
- Preserve formatting of selected identifier fields.
- Create working copies of the original data.
- Establish a consistent structure for downstream processing.

### 2. Data Cleaning and Preparation

- Standardize column names by converting them to lowercase and replacing non-alphanumeric characters with underscores.
- Simplify selected column names for easier reference.
- Preserve original values before applying transformations.
- Apply documented missing-value handling strategies where appropriate.
- Add missingness flags to support quality-assurance checks.
- Harmonize category names across both datasets using documented mappings.

### 3. Data Transformation

- Apply case normalization to relevant text fields.
- Remove unnecessary whitespace and selected special characters.
- Prepare selected fields for comparison across datasets.
- Create analytical variables where needed.
- Maintain reproducibility through documented functions and processing steps.

### 4. Cross-Referencing and Matching

- Create comparable subsets of both datasets.
- Apply a structured record-linkage workflow.
- Use broad, non-operational match categories to distinguish different levels of similarity.
- Separate strict, contextual, partial, and non-matching cases for further review.
- Avoid disclosing original operational rules, thresholds, or partner-specific matching logic.

### 5. Post-Matching Processing

- Run additional checks for records requiring manual review.
- Apply consistency checks to identify possible inconsistencies.
- Flag cases that require further validation.
- Preserve transparency around assumptions and processing decisions.

### 6. Final Data Preparation

- Reorganize columns for clarity and consistency.
- Merge matched records into a consolidated analytical structure.
- Prepare outputs for further analysis and internal reporting.

### 7. Exporting Results

- Export the final matched dataset to formats suitable for analysis and reporting.
- Specific outputs and findings remain confidential to the partner organization.

---

## Main Skills Used

### Data Analysis

- Structured data analysis with Python and pandas.
- Data inspection, transformation, and preparation for downstream analysis.

### Data Cleaning and Preparation

- Column-name standardization.
- Missing-value assessment and documentation.
- Text normalization.
- Category harmonization.
- Preservation of original values for auditability.

### Record Linkage

- Cross-referencing heterogeneous datasets.
- Designing a structured matching workflow.
- Separating strict, contextual, partial, and non-matching cases.
- Creating review flags for quality assurance.

### Reproducible Workflow

- Modular functions for repeatable processing.
- Jupyter Notebook documentation.
- Version control with Git.
- Clear separation between source data, processing logic, and analytical outputs.

### Responsible Data Practice

- Sanitization of public documentation.
- Use of synthetic or abstracted examples.
- Avoidance of sensitive operational details.
- Protection of partner confidentiality.

---

## Outputs

The pipeline produced a consolidated dataset that brought together two previously separate sources, enabling the partner NGO’s data team to examine patterns that were difficult to observe when the datasets were considered in isolation.

The work focused on:

- data quality;
- harmonization;
- record linkage;
- quality assurance;
- reproducible processing;
- documentation of assumptions.

Specific findings derived from the matched data remain confidential to the partner organization and are not included in this repository.

---

## Challenges and Solutions

### 1. Data Cleaning and Standardization

**Challenge:** The datasets came from different sources, with varying formats, column names, category labels, and data-entry conventions.

**Solution:** Standardized column names, preserved original values, applied consistent text normalization, harmonized category labels, and documented transformations.

### 2. Matching Across Heterogeneous Records

**Challenge:** Variations in how records were entered made cross-referencing non-trivial, with risks of both false matches and missed matches.

**Solution:** Implemented a structured matching workflow that separates strict, contextual, partial, and unmatched cases, allowing results to be reviewed according to their level of similarity.

### 3. Handling Missing and Incomplete Data

**Challenge:** Missing or incomplete fields can lead to inaccurate matching if not handled explicitly.

**Solution:** Applied documented missing-value handling strategies, added missingness flags, and avoided treating missing values as valid evidence of similarity.

### 4. Protecting Sensitive Information

**Challenge:** The project involved sensitive data and operationally relevant matching logic.

**Solution:** Created a sanitized public version using synthetic or abstracted examples. The repository documents the methodological structure without disclosing original datasets, field names, record counts, operational rules, thresholds, or findings.

---

## Technologies Used

- **Programming language:** Python
- **Libraries:** pandas, regular expressions (`re`)
- **Environment:** Jupyter Notebook
- **Version control:** Git / GitHub
- **Output formats:** Excel and CSV for internal analytical use

---

## Responsible Data Note

This project worked with data from a private source. To respect the confidentiality of the partner organization and the sensitivity of the domain, this repository does **not** include:

- the original datasets or any extracts of them;
- specific record counts;
- original field names or source-specific labels;
- record identifiers;
- operational matching rules or thresholds;
- partner-specific validation criteria;
- results or findings derived from the matched data.

The repository documents the analytical workflow, methodological choices, data-quality challenges, and reproducibility principles applied during the project.

The public notebook is a sanitized methodological version and should be understood as a portfolio demonstration of the workflow structure, not as a disclosure of the original operational pipeline.

---

## Conclusion

The project produced a reproducible pipeline to harmonize and match records across two heterogeneous datasets, with documented assumptions and responsible handling of sensitive policy data.

It demonstrates an applied approach to data cleaning, harmonization, record linkage, quality assurance, and reproducible analysis in a public-safety context.

---

## Next Steps

Potential future improvements include:

- refining quality-assurance checks;
- documenting additional data-validation procedures;
- exploring probabilistic record-linkage methods where appropriate;
- strengthening reproducibility through configuration files and automated tests;
- extending the methodology to additional complementary datasets, subject to partner needs and data-protection requirements;
- continuing collaboration with the partner NGO on refinements aligned with their analytical priorities.

---

## Files

- **[Notebook](./firearms_matching_system_sanitized.ipynb):** Sanitized methodological version of the workflow using synthetic or abstracted examples. Sensitive data, operational rules, thresholds, partner-specific details, and findings are not disclosed.
- **Data:** The original datasets cannot be shared because they come from a private source and include sensitive information.

---

## Contact

Feel free to reach out with questions or to discuss possible collaborations.

- **Email:** [tech.jbpeixo@gmail.com](mailto:tech.jbpeixo@gmail.com)
- **LinkedIn:** [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
- **GitHub:** [julianabpeixoto](https://github.com/julianabpeixoto)
