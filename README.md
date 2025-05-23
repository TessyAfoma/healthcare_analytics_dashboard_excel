# Healthcare Business Analysis

## Project Overview
This data analysis project is focused on providing insights into hospital operations using real-world data. By analysing patient trends, medical services, and financial trends, we intend to make data-driven decisions and recommendations and better understand the hospital's overall performance.

### Datasets Included
The analysis is based on 8 integrated datasets:
- **Patients**
- **Visits**
- **Providers**
- **Procedures**
- **Diagnoses**
- **Insurance**
- **Departments**
- **Cities**

Each dataset was cleaned, connected via lookup formulas, and consolidated into a **Master Sheet** for streamlined analysis.

### Tools
Microsoft Excel

### Data Cleaning/Preparation
To ensure accurate analysis and reporting, the following data cleaning and transformation steps were applied:

1. **Raw Data Consolidation**
- Imported data from 7 different Excel files into a single workbook with clearly labeled sheets: `Patients`, `Visits`, `Providers`, `Diagnosis`, `Procedure`, `Insurance`, `Cities`, and `Departments`.
- Created a central **Master Sheet** by joining all supporting data tables using `VLOOKUP`.

2. **Standardizing & Formatting**
- Ensured consistent column names (e.g., `Patient Name`, `Visit Date`, `Room Type`) across all sheets.
- Cleaned extra spaces, typos, and inconsistent text cases using `TRIM`, `LOWER`, and `PROPER` functions.
- Reformatted date columns to standard Excel date format for proper sorting and grouping.

3. **Handling Missing Data**
- Left blank `Follow-Up Visit Date` and `Admitted Date` cells untreated where appropriate (e.g., outpatient visits).
- Created logic-based columns (e.g., **Visit Type**) using formulas to classify data, even when some fields were blank.

4. **Data Transformation**
- Added calculated columns like:
  - `Visit Type` (Emergency vs. Scheduled)
  - `Is Follow-Up Visit` (Yes/No based on `Follow-Up Visit Date`)
  - `Revenue` (sum of `Treatment Cost` and `Medication Cost`)
  - `Month` and `Year` from `Visit Date` for trend analysis
- Converted `Yes`/`No` values in certain columns to consistent text categories (`Emergency`/`Scheduled`) for better chart visuals.

5. **Preparing for Analysis**
- Removed or excluded irrelevant blanks in PivotTables and charts to keep dashboards clean.
- Used slicers and filters to ensure dynamic interactivity across all dashboards.
- Built and hid source data sheets to keep the workbook focused and professional.

### Exploratory Data Analysis (EDA)
EDA involved exploring the data to answer these questions:

Who are the patients, and what are their characteristics?

What are the most common diagnoses and procedures, and how are providers performing?

How is the hospital performing financially, and where can costs be optimized?

### 📊 Key Dashboards

### 1 **Patient Demographics & Trends**
- Gender, age, and race distribution
- Top cities by patient count
- Follow-up visit frequency
- Satisfaction score by demographics

### 2 **Medical Services & Provider Performance**
- Most common diagnoses and procedures
- Department workloads
- Provider activity levels
- Provider-specialty alignment

### 3 **Financial & Operational Analysis**
- Total revenue from treatments and medications
- Inpatient vs outpatient breakdown
- Room type profitability
- Insurance coverage impact
- Emergency vs scheduled visit ratio

### 4 **Overview Dashboard**
- Executive summary of KPIs:
  - Total Patients
  - Total Revenue
  - Top Provider
  - Most Common Diagnosis
  - Avg Satisfaction Score
- Financial trendline by month
- Top contributing cities, providers and services

### Results 
The analysis results are summarized as follows:

The majority of patients come from Birmingham and Edinburgh, which together account for over 50% of total visits.

Hypertension is the leading diagnosis, indicating a potential focus area for preventive care.

Dr. Sade Kikiola sees the highest patient volume and generates the most revenue among providers.

January shows the highest number of patient visits, suggesting seasonal spikes in hospital activity.

### Recommendations
Based on the analysis
