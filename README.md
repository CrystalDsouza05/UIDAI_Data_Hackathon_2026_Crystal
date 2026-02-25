# UIDAI Hackathon 2026 – Aadhaar Enrolment & Update Analytics

## 📌 Project Overview

This project was developed as part of the **UIDAI Hackathon 2026**.

The objective of this analysis is to:

- Understand Aadhaar enrolment trends over time  
- Analyse demographic and biometric update patterns  
- Study age-wise distribution of Aadhaar activity  
- Examine geographic spread across states and districts  
- Perform monthly and Year-to-Date analysis  

The final output is an interactive Power BI dashboard that transforms raw UIDAI data into structured insights.


## Dashboard Images and Data Model

[Dashboard Link](https://app.powerbi.com/view?r=eyJrIjoiZmRmNTVmNTQtZWJiYi00NTRiLWFiZWYtNTQ1ZTNhNzJiZDMyIiwidCI6ImY3ODE3NzI4LWIzNTQtNGYwNi04ZmUzLTBiYzlmMzY4ZTRkYiJ9)

Page 1 - Adhaar Enrollment Dashboard Summary  
<img width="1280" height="720" alt="Slide1" src="https://github.com/user-attachments/assets/72f65760-e123-4166-a77e-3671ec606be5" />

Page 2 - Adhaar Enrollment Dashboard  
<img width="1280" height="720" alt="Slide2" src="https://github.com/user-attachments/assets/d2c0a6c3-7ae4-4de7-b7ab-93bbd0ab8e17" />

Page 3 - Adhaar Demographic Updates  
<img width="1280" height="720" alt="Slide3" src="https://github.com/user-attachments/assets/9f3018ea-f26e-4e65-9760-f10c509b8b55" />

Page 4 - Adhaar Bio-metric Updates  
<img width="1280" height="720" alt="Slide4" src="https://github.com/user-attachments/assets/04d98ed7-5bb8-47e0-824b-a83ea610a276" />

Data Model  
<img width="1280" height="720" alt="Slide5" src="https://github.com/user-attachments/assets/b84b8d7b-f3aa-4185-9b24-605bb430c1d2" />



## 📂 Datasets Used

Three official UIDAI datasets were used:

### 1️⃣ Aadhaar Enrolment Data
- Date  
- State  
- District  
- Pin Code  
- Enrolments by Age Group (0–5, 5–17, 18+)  

### 2️⃣ Aadhaar Demographic Update Data
- Date  
- State  
- District  
- Pin Code  
- Updates for Age Groups (5–17, 17+)  

### 3️⃣ Aadhaar Biometric Update Data
- Date  
- State  
- District  
- Pin Code  
- Biometric updates for Age Groups (5–17, 17+)  

All three datasets followed a similar structure, enabling combined analysis.

## 🧹 Data Preparation and Transformation

### 📥 Data Loading
- Used folder connection in Power BI  
- Combined multiple API files automatically  
- Removed hidden and system files  

### 🧽 Data Cleaning
- Applied correct data types  
- Standardised inconsistent state names  
  - Westbengal → West Bengal  
  - Orissa → Odisha  
  - Tamilnadu → Tamil Nadu  
- Removed extra spaces and inconsistencies  

This ensured accurate geographic analysis and avoided duplicate state entries.

### 🔄 Age Group Transformation
- Unpivoted age group columns  
- Created a unified `AgeGroup` column  
- Created a `Citizens` value column  

This allowed consistent analysis across enrolments and updates.

### 📅 Date Table Creation
A separate Date table was created to support:

- Monthly trend analysis  
- Year-to-Date calculations  
- Month-over-Month comparison  
- Proper chronological month sorting  

Note: August does not appear in visuals due to absence of records in the source data.

## 📊 Key Metrics

- Total Enrolments: 5,435,702  
- Total Demographic Updates: 49,295,187  
- Total Biometric Updates: 69,763,095  

Update activities are significantly higher than new enrolments, indicating continuous maintenance of Aadhaar records.

## 🔎 Key Insights

### 👥 Age Group Analysis

**Enrolments**
- Highest activity in 0–5 age group  
- Lower enrolments in 18+ group  

**Demographic Updates**
- Majority from 17+ age group  

**Biometric Updates**
- High activity in both 5–17 and 17+ groups  


### ⏳ Time-Based Trends

- Steady monthly increase  
- Clear cumulative Year-to-Date growth  
- Operational variation across months  

YTD analysis helps evaluate overall performance rather than isolated monthly figures.


### 🗺 Geographic Insights

- High activity in Uttar Pradesh, Maharashtra, Bihar, and Madhya Pradesh  
- Activity correlates with population size  
- District-level variation observed  
- Daily averages used for fair state comparison  


## 🏗 Data Model Structure

The model includes:

- Date table  
- Enrolment fact table  
- Demographic update fact table  
- Biometric update fact table  
- Structured relationships for time intelligence  

This supports clean filtering and structured analysis.


## 🛠 Tools and Skills Demonstrated

- Power BI  
- Power Query  
- Data Cleaning and Standardisation  
- Data Transformation  
- Date Table Creation  
- Time Intelligence  
- Dashboard Design  
- Geographic Analysis  


## 🎯 Conclusion

This project demonstrates how structured data cleaning, transformation, and modeling can convert raw public datasets into meaningful analytical insights.

The dashboard provides a clear and structured view of Aadhaar enrolments and updates across age groups, time periods, and geographic regions in India.


Author: Crystal Andrea Dsouza  
TYBAF Student, St. Xavier’s College, Mumbai  

