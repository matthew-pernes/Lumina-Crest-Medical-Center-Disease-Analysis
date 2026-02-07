# Lumina-Crest-Medical-Center-Disease-Analysis

<img width="1697" height="644" alt="image" src="https://github.com/user-attachments/assets/c0d11265-017c-491d-a488-662f53ffab4c" />

## Project Overview & Business Problem

This project analyzes patient demographics, disease prevalence, and billing at **Lumina Crest Medical Center** via an interactive Excel dashboard. By segmenting data by age and diagnosis, it identifies key trends in healthcare utilization and insurance costs. These insights help stakeholders optimize hospital resource allocation and financial planning.

**Business Problem:** Hospital administrators struggled to visualize the relationship between patient demographics and rising treatment costs, making it difficult to predict budget needs and staffing requirements for high-demand age groups.

**Solution Created:**
I developed an interactive Excel dashboard that centralizes complex clinical data into four dynamic visualizations. To ensure high usability, I integrated **Slicers** for **Medical Condition, Age Bracket, and Gender**, allowing users to filter the following insights instantly:

* **Blood Type per Gender:** Distribution analysis for blood bank inventory planning.
* **Medications per Age Group:** Correlation between patient age and pharmaceutical requirements.
* **Average Billing per Insurance Provider:** Financial breakdown to identify high-revenue and high-cost partnerships.
* **Diseases per Age Group:** Epidemiological trends to assist in specialized department staffing.

## 2. Data Dictionary & Sources

The dataset used for this analysis was sourced from **Kaggle** and contains synthetic patient records designed to mirror real-world hospital data.

* **Dataset Source:** [Kaggle Healthcare Dataset]
* **File Name:** The raw data is available in this repository as `healthcare_dataset.csv`.

Data Dictionary

| Column | Description |
| :--- | :--- |
| **Name** | Patient's full name |
| **Age** | Age of the patient at the time of admission |
| **Gender** | Patient's gender (Male/Female) |
| **Blood Type** | Patient's blood group (e.g., A+, O-, etc.) |
| **Medical Condition** | The primary diagnosis (e.g., Diabetes, Asthma, Hypertension) |
| **Date of Admission** | The date the patient was admitted to the facility |
| **Doctor** | The name of the attending physician |
| **Hospital** | The specific facility (Lumina Crest Medical Center) |
| **Insurance Provider** | The company covering the patient's medical expenses |
| **Billing Amount** | The total cost of the hospital stay (USD) |
| **Room Number** | The assigned room for the patient's stay |
| **Admission Type** | Category of admission (Emergency, Elective, Urgent) |
| **Discharge Date** | The date the patient left the hospital |
| **Medication** | The primary medication prescribed during the stay |
| **Test Results** | The outcome of clinical tests (Normal, Abnormal, Inconclusive) |
