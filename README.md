# AI-Driven Healthcare Analytics: Optimizing Patient Flow and Satisfaction 🏥📊

## 📌 Project Overview
Currently, healthcare facilities struggle with managing patient flow, leading to prolonged wait times and decreased patient satisfaction. This project provides a data-driven solution to monitor wait times across various departments, identify operational bottlenecks, and ensure efficient healthcare delivery. 

By leveraging data analytics and visualization, this project translates raw hospital records into an interactive monitoring system, allowing administrators to make informed decisions on resource allocation and staffing.

**Note:** This project was developed as a Capstone Project for the MS Elevate AICTE Internship.

## 🛠️ Tech Stack
* **Data Preprocessing & Analysis:** Python (Pandas, NumPy)
* **Business Intelligence & Visualization:** Microsoft Power BI
* **Data Expressions:** DAX (Data Analysis Expressions)

## 📂 Dataset Details
The analysis is based on a healthcare dataset comprising over 9,200 patient records. Key features include:
* `date` & `Moment` (AM/PM)
* `patient_id`, `patient_age`, `patient_gender`, `patient_race`
* `patient_waittime` (in minutes)
* `department_referral` (e.g., General Practice, Cardiology, Orthopedics)
* `patient_sat_score` (1-10 scale)
* `patient_admin_flag` (Admission status)

## ⚙️ Project Workflow

### 1. Data Preprocessing (Power Query Editor)
Before visualization, the raw dataset required cleaning to ensure data integrity:
* **Handling Missing Values:** Applied data imputation techniques to address null values in the `patient_sat_score` and `department_referral` columns.
* **Anomaly Detection:** Identified and managed outliers in the `patient_waittime` feature to prevent skewed averages.
* **Feature Engineering:** Segmented patient traffic patterns by time of day to uncover peak operational hours.

### 2. Interactive Power BI Dashboard
The cleaned dataset was imported into Power BI to construct a dynamic, interactive dashboard featuring 6 primary visualizations:
1. **Patient Volume Trend (Line Chart):** Tracks daily hospital inflow to identify busy seasons.
2. **Average Wait Time by Department (Clustered Bar Chart):** Pinpoints the exact departments keeping patients waiting the longest.
3. **Patient Demographics (Stacked Column Chart):** Displays demographic breakdowns (Race/Gender).
4. **Wait Time vs. Satisfaction (Scatter Chart):** Analyzes the correlation between prolonged wait times and declining patient satisfaction scores.
5. **Hospital Traffic by Time of Day (Donut Chart):** Highlights AM vs. PM operational volume.
6. **Average Satisfaction by Department (Gauge Chart):** Dynamic gauges synced with a slicer to measure if individual departments are meeting the target hospital satisfaction score (8/10).

## 🚀 Future Scope
* **IoT Integration:** Incorporating real-time IoT sensor data from hospital beds or wearable devices to provide a live feed of hospital capacity.
* **Cloud Architecture:** Deploying the data pipeline on a cloud platform (AWS/Azure) to allow multiple hospital branches to sync their data centrally for cross-regional analysis.
* **Predictive Modeling:** Implementing machine learning algorithms (e.g., Random Forest) to predict anticipated wait times based on historical trends before a patient arrives.

## 💻 How to Run the Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/healthcare-analytics-dashboard.git](https://github.com/your-username/healthcare-analytics-dashboard.git)
