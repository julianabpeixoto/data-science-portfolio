# Arsenal do Crime — Seized Firearms in Southeast Brazil, 2018–2023

**Instituto Sou da Paz · Public safety · Firearms policy · Data automation · Published report**

## Table of Contents

1. [Project at a Glance](#project-at-a-glance)
2. [Project Context](#project-context)
3. [My Contribution](#my-contribution)
4. [Data Challenges](#data-challenges)
5. [Analytical Workflow](#analytical-workflow)
6. [Responsible Data Note](#responsible-data-note)
7. [Outputs](#outputs)
8. [Main Skills Demonstrated](#main-skills-demonstrated)
9. [Why This Project Matters](#why-this-project-matters)
10. [Published Report](#published-report)
11. [Contact](#contact)

---

## Project at a Glance

* **Role:** Credited contributor to a published NGO research report
* **Organization:** Instituto Sou da Paz
* **Domain:** Public safety, firearms policy, illicit firearms markets
* **Geographic scope:** Southeast Brazil
* **Time period analyzed in the report:** 2018–2023
* **Main task:** Data cleaning, harmonization, analytical variable construction, and automation
* **Core methods:** Data cleaning, data harmonization, rule-based classification, reproducible workflow, documentation
* **Tools:** Python, pandas, spreadsheet-based data review, documentation
* **Data access:** Restricted; original data and operational rules are not shared in this repository

---

## Project Context

*Arsenal do Crime: Análise do perfil das armas de fogo apreendidas no Sudeste, 2018–2023* is a report published by Instituto Sou da Paz analyzing the profile of firearms seized in Southeast Brazil between 2018 and 2023.

The report contributes to the public debate on firearms circulation, illicit markets, regulatory changes, and evidence-based public safety policies.

This case study documents my contribution to the data preparation stage of the project, focusing on data quality, harmonization, traceability, and automation.

---

## My Contribution

My work focused on the second stage of data preparation and analytical enrichment.

I contributed to:

* cleaning and harmonizing firearm-related data;
* structuring analytical variables used in the report;
* extending a Python automation script to infer firearm manufacturing year from serial-number patterns;
* applying the method to **Boito** and **CBC** firearms, building on prior work developed for Taurus-manufactured firearms;
* improving consistency, traceability, and scalability in the analytical pipeline.

This work supported the broader research team in generating evidence on the temporality, profile, and circulation dynamics of seized firearms.

---

## Data Challenges

The dataset required careful preparation because administrative and government datasets in public safety contexts often present inconsistencies, missing values, heterogeneous formats, and incomplete classification fields.

Key challenges included:

* inconsistent or incomplete firearm identification fields;
* variation in manufacturer-related information;
* need to preserve traceability of analytical decisions;
* need to avoid manual, non-reproducible classification procedures;
* sensitivity of the source data and analytical rules.

The project required balancing analytical usefulness with responsible handling of sensitive information.

---

## Analytical Workflow

The workflow included the following stages:

### 1. Data Review and Cleaning

* Reviewed relevant firearm identification fields.
* Checked consistency across manufacturer, model, and serial-number information.
* Identified fields requiring harmonization or analytical enrichment.

### 2. Variable Structuring

* Supported the construction and review of analytical variables.
* Ensured that variables used in downstream analysis were consistent and interpretable.
* Helped improve the usability of the dataset for descriptive analysis and reporting.

### 3. Automation Script Extension

* Extended an existing Python-based approach to infer firearm manufacturing year from serial-number patterns.
* Applied the method to additional manufacturers, specifically Boito and CBC.
* Structured the logic to improve reproducibility and reduce manual classification work.

### 4. Quality and Traceability

* Supported consistency checks in the analytical pipeline.
* Helped ensure that assumptions and transformations could be reviewed and traced.
* Contributed to a more scalable approach for handling firearm identification data.

---

## Responsible Data Note

This repository does **not** include:

* the original dataset;
* any extracts of the source data;
* operationally sensitive classification rules;
* serial-number logic or thresholds;
* intermediate or final analytical datasets;
* confidential findings not disclosed in the published report.

This page is a methodological case study. Its purpose is to document the type of analytical contribution, data-quality challenges, and responsible data practices involved in the project without exposing sensitive information.

---

## Outputs

The work contributed to the data preparation and analytical pipeline underpinning the published report.

The main outputs of my contribution were:

* improved harmonization of selected firearm-related fields;
* structured analytical variables;
* extended automation logic for manufacturing-year inference;
* improved consistency and traceability in the data preparation process;
* support to a published NGO research report on seized firearms in Southeast Brazil.

---

## Main Skills Demonstrated

### Data Cleaning and Harmonization

Prepared and reviewed complex administrative data, with attention to consistency, missingness, and analytical usability.

### Analytical Variable Construction

Supported the creation and refinement of variables used to analyze firearm profiles, temporality, and circulation patterns.

### Python Automation

Extended a Python automation script to reduce manual work and improve reproducibility in the classification process.

### Data Quality Assurance

Contributed to consistency checks, traceability, and methodological transparency in the analytical workflow.

### Responsible Data Use

Documented the project in a way that preserves confidentiality and avoids disclosure of sensitive operational details.

### Public Policy Analysis

Contributed to a research product designed to inform public debate and evidence-based recommendations on firearms policy and public safety.

---

## Why This Project Matters

This project demonstrates how data science can support public-interest research in sensitive policy areas.

In practical terms, it shows how data cleaning, harmonization, automation, and documentation can help transform complex administrative records into more reliable evidence for analysis, reporting, and policy recommendations.

It also illustrates the importance of responsible data practices when working with sensitive public safety datasets.

---

## Published Report

The full report is available on the Instituto Sou da Paz website:

[Arsenal do Crime: Análise do perfil das armas de fogo apreendidas no Sudeste, 2018–2023](https://soudapaz.org/documentos/arsenal-do-crime-analise-do-perfil-das-armas-de-fogo-apreendidas-no-sudeste-2018-2023/)

---

## Contact

Feel free to reach out with questions or to discuss possible collaborations.

* **Email:** [jbertolucci@gmail.com](mailto:jbertolucci@gmail.com)
* **LinkedIn:** [Juliana Bertolucci Peixoto](https://www.linkedin.com/in/julianabpeixoto)
* **GitHub:** [julianabpeixoto](https://github.com/julianabpeixoto)
