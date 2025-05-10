# 📊 Google Play Store Analytics Dashboard

This project is part of my Data Analyst internship at NullClass. It focuses on building an interactive, real-time dashboard that visualizes Google Play Store data using Python, Pandas, Plotly, and Dash. The dashboard provides insights into app trends, user reviews, and ratings through multiple visualizations with time-based logic.

---

## 🚀 Live Demo

🔗 **Dashboard:** [https://googleplay-dashboard.netlify.app/](https://googleplay-dashboard.netlify.app/)

---

## 📝 Project Overview

The goal of this project was to extract insights from Google Play Store data and present them in a dynamic and interactive dashboard. The dashboard includes:

- ✅ Word Cloud from 5-star reviews in the **Health & Fitness** category.
- ✅ Grouped Bar Chart comparing top categories by installs and review metrics (with **time-controlled visibility** between 3 PM – 5 PM IST).
- ✅ Bubble Chart analyzing the relationship between app size and rating (visible only between 5 PM – 7 PM IST).

---

## 📂 Repository Contents

- `null_classes_tasks.ipynb` – Main Jupyter Notebook with code for data cleaning, processing, and visualization.
- `requirements.txt` – Python dependencies.

---

## 🛠 Technologies Used

- **Python 3.x**
- **Pandas**
- **Plotly Express**
- **Dash (for interactive dashboard)**
- **NLTK (for text processing)**
- **WordCloud**
- **Matplotlib**
- **Netlify (for hosting the dashboard)**

---

## ✨ Features

- 📊 **Word Cloud:** Highlights common positive keywords from 5-star reviews in Health & Fitness apps.
- 🗂️ **Grouped Bar Chart:** Displays average ratings and total review counts for the top 10 app categories based on installs.
- 🔵 **Bubble Chart:** Visualizes the relationship between app size (MB) and rating, with bubble size representing installs.
- ⏰ **Time-Based Rendering:** Certain visualizations are visible only during specific IST time slots for dynamic control.
- 📈 **Data Cleaning & Preprocessing:** Handled inconsistent data (e.g., "Size", "Installs", and "Last Updated" columns).

---

## 📊 Visualizations

| Visualization                           | Description                                                                                   |
|----------------------------------------|-----------------------------------------------------------------------------------------------  |
| Word Cloud                              | 5-star reviews (Health & Fitness) after stopword and app name removal                          |
| Grouped Bar Chart                       | Average rating & review count for top categories (3 PM – 5 PM IST)                              |
| Bubble Chart                            | Size vs Rating (Bubble = Installs) for selected categories (5 PM – 7 PM IST)                   |

---

## ✅ Tasks Completed

- **Dataset Cleaning:**
  - Cleaned `Installs`, `Size`, and `Last Updated` columns.
  - Converted data types and handled missing/inconsistent values.

- **Word Cloud Generation:**
  - Filtered 5-star reviews in Health & Fitness.
  - Removed stopwords and app names before visualization.

- **Grouped Bar Chart:**
  - Aggregated data by category.
  - Applied filters: Rating ≥ 4.0, Size ≥ 10 MB, Last Updated in January.

- **Bubble Chart:**
  - Filtered: Rating > 3.5, Reviews > 500, Sentiment Subjectivity > 0.5, Installs > 50k.
  - Selected categories: Game, Beauty, Business, Comics, Communication, Dating, Entertainment, Social, Event.

- **Dashboard Integration:**
  - Modular layout with Dash.
  - Time-based conditional rendering.

---

## 🔍 Challenges Faced & Solutions

| **Challenge**                                         | **Solution**                                                                                                  |
|-------------------------------------------------------|--------------------------------------------------------------------------------------------------------------|
| Mixed data types in "Size" and "Installs" columns     | Cleaned using regex and `pd.to_numeric(errors='coerce')` to handle inconsistencies                            |
| Inconsistent date formats in "Last Updated"           | Applied `pd.to_datetime(errors='coerce')` for uniform datetime conversion                                     |
| Time-based chart visibility logic                     | Used `datetime.now(pytz.timezone('Asia/Kolkata'))` to enable dynamic chart display within time ranges         |
| Word Cloud not rendering due to preprocessing issues  | Improved data cleaning (stopwords, app name removal) and ensured non-empty text input                         |

---

## 🙌 Acknowledgments

Thanks to **NullClass** for providing the opportunity to work on this internship project and for the structured training and support.

---
