# 💼 Job Salary Analysis (Excel)

An Excel project that analyses a **250,000-record job salary dataset** to find out which factors influence pay: job title, experience, education, industry, location, company size, remote work, skills and certifications. The analysis uses Pivot Tables, calculated columns and charts on a dashboard sheet.

---

## 📌 Project Overview

Salary data is only useful when you can see what drives it. This project summarises a large salary dataset with Pivot Tables and visualises the results to answer questions such as:

- How does salary change with years of experience?
- Which job titles and education levels earn the most?
- Does industry, company size or location make a real difference?
- Do remote work, skills and certifications affect pay?

## 🖼️ Dashboard Preview

> Add screenshots to an `images/` folder and update the paths below.

[Dashboard]

## 📂 Dataset

**Sheet:** `job_salary_prediction_dataset`
**Size:** 250,000 rows × 10 columns, with no missing values

| Column | Description |
|---|---|
| job_title | Role of the employee (12 job titles, for example AI Engineer, Data Analyst) |
| experience_years | Years of experience (0 to 20) |
| education_level | High School, Diploma, Bachelor, Master or PhD |
| skills_count | Number of skills listed |
| industry | Industry the company belongs to (10 industries) |
| company_size | Startup, Small, Medium, Large or Enterprise |
| location | Country or Remote |
| remote_work | Yes, Hybrid or No |
| certifications | Number of certifications (0 to 5) |
| salary | Annual salary (the dataset does not specify a currency) |

**Calculated column:** `Experience` = `IF(experience_years > 5, "Expert", "Novice")`

## 📑 Workbook Structure

| Sheet | Purpose |
|---|---|
| **Chart1** | Standalone chart sheet |
| **PVT** | Pivot Tables that summarise average salary by experience, job title, education level and industry |
| **job_salary_prediction_dataset** | Raw dataset with the calculated `Experience` column |
| **DB** | Dashboard sheet with the charts |

## 📊 Charts

| Chart | Type | Shows |
|---|---|---|
| Salary vs Experience | Bar chart | Average salary for each year of experience |
| Salary by Job Title | Pie chart | Salary comparison across job titles |
| Average Salary by Education Level | Doughnut chart | Average salary for each education level |
| Average Salary in Each Industry | Line chart | Average salary across industries |

## 🔍 Key Findings

These figures come from the full 250,000-row dataset.

- **Overall average salary** is about **145,718**, with a median of 143,453.
- **Experience matters most.** Average salary rises steadily from about **118,873** at 0 years to about **173,180** at 20 years. "Expert" (more than 5 years) employees average about **153,835**, against **125,462** for "Novice".
- **Job title:** AI Engineer earns the most on average (about **173,498**), followed by Machine Learning Engineer (**163,023**) and Product Manager (**157,595**). Data Analyst (**119,892**) and Business Analyst (**122,551**) are at the lower end.
- **Education:** pay increases with each level, from about **131,715** (High School) to about **163,976** (PhD).
- **Location:** USA has the highest average (about **181,716**) and India the lowest (about **97,690**).
- **Company size:** Enterprise companies pay about **169,616** on average, against about **127,289** at startups.
- **Industry makes almost no difference.** Industry averages sit within a narrow range of about 145,400 to 146,000, so industry is a weak driver of salary here.
- **Certifications:** average salary rises with every additional certification, from about **141,492** (none) to about **149,607** (five).
- **Remote work:** fully remote roles average about **149,280**, slightly above Hybrid and On-site (about 144,000).

## 🛠️ Skills Demonstrated

- Pivot Tables and Pivot Charts
- Data summarisation and aggregation (Average of salary)
- Calculated columns using `IF` and `GETPIVOTDATA`
- Data visualisation (bar, pie, doughnut and line charts)
- Working with a large dataset (250K rows)

## ▶️ How to Use

1. Download or clone this repository.
2. Open `DB.xlsx` in **Microsoft Excel**.
3. Go to the **PVT** sheet to see the Pivot Tables, and the **DB** sheet for the dashboard.
4. Right-click a Pivot Table and choose **Refresh** after changing the data.

> ⚠️ The file is large (about 26 MB) because of the 250K-row dataset and the Pivot cache, so it may take a moment to open.

## 📁 Repository Structure

```
job-salary-analysis-excel/
├── Excel-Dashboard.xlsx          # Excel workbook (dataset, pivots, charts, dashboard)
├── images/          # Dashboard screenshots
└── README.md
```

## 👩‍💻 Author

**Jasmin P P**
Aspiring Data Analyst | Thrissur, India

[LinkedIn]
