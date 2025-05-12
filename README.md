# LA_Crime

# 🕵️‍♂️ Los Angeles Crime Data Analysis (2020 - Present)

This project explores and visualizes the Los Angeles Crime dataset from 2020 to the present. The dataset includes detailed records of crime incidents, including location, time, victim demographics, weapon type, and more. The main goal of this project was to clean the data, perform feature engineering, carry out EDA, and use unsupervised clustering (K-Means) to identify patterns in the data.


## 📊 Dataset Overview

- **Source:** City of Los Angeles Open Data
- **Records:** 1+ million crime reports
- **Time Range:** 2020 to Present
- **Features include:**
  - Crime type and description
  - Location data (LAT, LON, Area Name)
  - Time of occurrence (hour, date, month)
  - Victim info (age, gender, descent)
  - Weapon info, status codes, premises type
  - 

## 🧹 Data Cleaning & Preprocessing

- Removed or filled missing values using appropriate strategies:
  - Categorical fields like `Vict Sex`, `Vict Descent`, and `Weapon Desc` filled with `'Unknown'`
  - Numerical fields like `Vict Age` preserved
- Converted `DATE OCC` and `Date Rptd` to datetime objects
- Extracted:
  - `Hour` from `TIME OCC`
  - `Month` and `Year` from `DATE OCC`
- Added a `DATETIME OCC` column for full timestamp



## 📈 Exploratory Data Analysis (EDA)

### 🔍 Time-based Patterns
- Crime frequency by **hour of the day**
- Monthly and yearly trends
- Heatmap of **crime distribution by Hour vs. Month**

### 📍 Location-based Patterns
- Top areas with the highest crime frequency
- Crime density visualized using scatter plots over LAT/LON

### 🚻 Demographics
- Victim age distribution
- Crime counts by **victim gender** and **descent**

### 🔫 Crime and Weapons
- Most common crime types (`Crm Cd Desc`)
- Most frequently used weapons
- Bar charts for part 1 vs part 2 crimes (`Part 1-2`)


## 📦 Libraries Used

- `pandas`, `numpy`
- `matplotlib`, `seaborn`


## 📌 Notes

- No supervised ML model was built since the dataset lacked a proper target variable.
- Focus was on building insight from raw public data using classic data analysis workflows.

