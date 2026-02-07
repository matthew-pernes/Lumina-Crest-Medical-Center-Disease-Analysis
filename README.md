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

* **Dataset Source:** [[Kaggle Healthcare Dataset]](https://www.kaggle.com/datasets/prasad22/healthcare-dataset)
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

## 3. Data Cleaning & Transformation

Data integrity is crucial in healthcare analytics. Before building the dashboard, I performed the following cleaning steps in Excel to ensure the dataset was accurate and ready for analysis:

* **Standardized Name Formatting:** Used the `PROPER` function and removed leading/trailing spaces to ensure patient names were consistent across the 10,000+ records.
* **Created Age Brackets:** Used a nested `IF` statement (or `IFS`) to categorize patients into demographic groups (e.g., 0-17, 18-34, 35-64, 65+). This allowed for more meaningful trend analysis than individual ages.
* **De-duplication:** Performed a systematic check for duplicate patient IDs and records using Excel's **Remove Duplicates** tool to ensure the billing totals were not artificially inflated.
* **Data Type Validation:** Verified that 'Billing Amount' was formatted as Currency and 'Admission/Discharge' dates were formatted correctly to enable time-series calculations.

## 4. Key Insights & Visualizations

The **Lumina Crest Interactive Dashboard** allows for real-time exploration of hospital performance. Below are the primary insights discovered during the analysis:

* **Insurance & Revenue:** Analysis of **Average Billing per Insurance Provider** revealed that Medicare and Blue Cross Blue Shield have a higher average billing cost, suggesting a higher concentration of intensive care cases or specific elective procedures within those networks.
* **Demographic Demand:** By using the **Age Bracket** slicer, data shows that the 35-64 age group represents the highest volume of patients for across all diseases, directly correlating to a higher demand for specific maintenance medications.
* **Resource Allocation:** The **Medications per Age Group** chart identifies that pediatric patients (0-17) are most frequently prescribed Ibuprofen and Lipitor, while the 65+ bracket shows a sharp demand for Aspirin and Ibuprofen, signaling a need for more concentrated pharmacy inventory for seniors.
* **Clinical Distribution:** The **Blood Type per Gender** visualization confirms a balanced distribution, ensuring that the hospital’s blood bank inventory levels are currently aligned with the patient population's biological needs.

> **Note:** To view these insights dynamically, use the slicers located on the left-hand side of the `Dashboard` sheet in the provided `.xlsx` file.

## 5. Conclusion & Recommendations

The analysis of the Lumina Crest dataset highlights a clear correlation between patient age demographics and financial outcomes. By utilizing the interactive dashboard, the hospital can shift from reactive management to proactive resource planning.

# Strategic Recommendations:
* **Targeted Pharmacy Inventory:** Since the 35-64 age bracket shows the highest volume in medication needs, the hospital should optimize supply chain contracts for chronic disease medications (e.g., obesity and diabetes treatments) to reduce procurement costs.
* **Insurance Contract Review:** With significant variance in **Average Billing per Provider**, the finance department should investigate why specific providers show higher costs to ensure reimbursement rates are aligned with the complexity of care provided.
* **Specialized Care Staffing:** The data indicates high utilization rates for Obesity and Diabetes within the middle-age demographics. Lumina Crest should consider increasing specialized nursing staff during peak admission periods identified in the seasonal data.
* **Future Scaling:** To improve this analysis, I recommend integrating a "Length of Stay" metric in future iterations to calculate the direct correlation between bed occupancy and total billing efficiency.

---
**Technical Note:** This project demonstrates proficiency in Excel data modeling, Visualization, and data interpretation for business dashboards.
