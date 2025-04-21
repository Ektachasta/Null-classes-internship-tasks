# Google Play Store Analytics Dashboard 📊

This repository contains the source code and analysis for my Data Analyst internship project at NullClass. The project involves real-time analytics on Google Play Store data using Python, focusing on interactive visualizations and time-based logic integration using Plotly and Dash.

---

## 📌 Introduction

This internship project aims to explore, analyze, and visualize Google Play Store data to derive meaningful insights using Python. The focus is on mastering data preprocessing, visualization libraries like Plotly, and deploying dashboards.

---

## 🧠 Background

The project is built around a dataset of Google Play Store apps and user reviews. By combining data manipulation with powerful visualizations, this project simulates a real-world data analytics task that prepares interns for industry-level challenges.

---

## 🎯 Learning Objectives

- To clean, filter, and transform structured datasets using Python and Pandas.
- To create interactive and conditional visualizations using Plotly and Dash.
- To generate actionable insights from user reviews and app metrics.
- To host dashboards and manage version control using Git and GitHub.

---

## 📋 Activities and Tasks

### ✅ Completed:
- Word Cloud Generation from 5-star reviews (Health & Fitness category).
- Grouped Bar Chart comparing top categories by installs and review metrics (time-controlled visibility).
- Dataset cleaning, formatting, and filtering (Installs, Size, Last Updated).
- Dash layout integration for hosting multiple graphs.
  
---

## 🛠 Skills and Competencies Gained

- Data cleaning and preprocessing (handling nulls, formatting columns).
- Filtering and grouping using Pandas.
- Plotly for dynamic, interactive visualizations.
- Conditional rendering with datetime and Dash.
- GitHub project management and version control.

---

## 🔍 Feedback and Evidence

Progress throughout the internship has been documented consistently through screenshots and shared regularly with the mentor for evaluation. Key feedback received included:

- Enhancing layout structure and component alignment using Dash.  
- Resolving data type issues during preprocessing and transformation stages.  
- Applying precise filtering logic before generating visualizations.  

🔗 **Live Dashboard:** [Google Play Store Analytics Dashboard](https://googleplay-dashboard.netlify.app/)

---

## ⚠️ Challenges and Solutions

| Challenge | Solution |
|----------|----------|
| Handling mixed data types in "Size" and "Installs" columns | Used regex and replacement logic with Pandas to standardize them |
| Filtering by “Last Updated” with inconsistent formats | Applied `pd.to_datetime()` with `errors='coerce'` |
| Display logic based on time (IST) | Implemented `datetime.now(pytz.timezone(...))` logic inside Dash callback |
| Word cloud not rendering initially | Ensured data cleaning was applied properly before plotting |

---

## 🧾 Outcomes and Impact

- Developed an end-to-end analytical dashboard.
- Strengthened practical knowledge of data analytics workflows.
- Improved understanding of time-based event handling in visualizations.
- Contributed towards confidence in using GitHub for project deployments.

---

## ✅ Conclusion

The internship has been a valuable experience in bridging the gap between theoretical knowledge and practical implementation. By working with real-world datasets and tools, I’ve enhanced my problem-solving, visualization, and data storytelling skills.

---

