# 💼 Job Listings Dataset Analysis

This repository contains a cleaned and processed dataset of job listings with key company and job-related features such as salary, rating, company age, and location. The data was preprocessed using Python and Pandas for further analysis and visualization.

## 📁 Dataset Overview

The dataset includes the following columns:

| Column Name     | Description                                                                 |
|------------------|-----------------------------------------------------------------------------|
| `Index`          | Unique identifier for each row (auto-generated).                           |
| `Age`            | Age of the company (derived from the year it was established).             |
| `Salary`         | Offered salary for the job (cleaned and converted to float).               |
| `Rating`         | Company or job rating (typically on a 0–5 scale).                          |
| `Location`       | City or region where the job is located.                                   |
| `Established`    | Year when the company was founded.                                          |
| `Easy Apply`     | Indicates whether the job supports quick apply (Yes/No, converted to bool).|

---

## 🧹 Data Cleaning and Transformation

The following steps were taken to prepare the data:

- Removed currency symbols (`$`, `K`, etc.) from the `Salary` column.
- Converted `Salary` and `Rating` columns to numeric format.
- Derived the `Age` column using the formula: `Age = Current Year - Established`.
- Transformed `Easy Apply` column into boolean values (`Yes` → `True`, `No` → `False`).
- Removed unnecessary or redundant columns like `Index` if not required.

---

## 📊 Potential Use Cases

You can use this cleaned dataset for:

- 📍 Visualizing top locations for jobs with "Easy Apply"
- 💵 Analyzing salary distribution based on job rating
- 🧠 Understanding how company age affects job rating or salary
- 📈 Correlation between various job attributes
- 🤖 Building machine learning models for job recommendation

---

## 🧪 How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/SwathyKrishna02/job-listings-analysis.git
   cd job-listings-analysis

