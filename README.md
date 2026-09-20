# 🎬 Movie Analytics Dashboard

## 📌 Project Overview

**Movie Analytics Dashboard** is a data analytics and visualization project that analyzes movie data based on **genre, ratings, budget, revenue, profit, ROI, and release year**.

The project uses **Python and Pandas** for data cleaning and preparation and **Microsoft Power BI** to create an interactive dashboard that helps users explore movie performance and trends.

---

## 🎯 Objectives

- Analyze movies across different genres.
- Understand movie rating patterns.
- Analyze budget and revenue.
- Calculate movie profit and ROI.
- Identify top-performing movies.
- Analyze movie releases over the years.
- Build an interactive Power BI dashboard.
- Present movie data through clear and meaningful visualizations.

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Data cleaning and preprocessing |
| 🐼 Pandas | Data manipulation |
| 🔢 NumPy | Numerical operations |
| 📊 Matplotlib | Exploratory visualization |
| 📈 Power BI | Interactive dashboard |
| 📗 Excel | Data storage and analysis |
| 🧮 DAX | Power BI measures |
| 🐙 GitHub | Project version control |

---

## 📂 Dataset

The project uses the **TMDB 5000 Movie Dataset**, containing information about thousands of movies, including:

- Movie title
- Budget
- Revenue
- Genres
- Release date
- Runtime
- Popularity
- Vote average
- Vote count
- Original language
- Production information

The cleaned dataset contains **4,803 movies**.

---

## 🔄 Project Workflow

```text
Raw TMDB Dataset
       ↓
Data Loading
       ↓
Data Cleaning
       ↓
Data Preprocessing
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Power BI Data Preparation
       ↓
DAX Measures
       ↓
Interactive Dashboard
       ↓
Insights & Analysis

🧹 Data Preprocessing

The dataset was cleaned and prepared using Python.

Major preprocessing steps include:

Handling missing values
Removing duplicate movie IDs
Converting numeric columns to appropriate data types
Converting release dates
Extracting release year
Handling invalid budget and revenue values
Calculating profit
Calculating ROI
Creating rating categories
Extracting individual genres
Preparing separate genre analysis tables
📐 Calculated Metrics

Profit

Profit = Revenue - Budget

ROI

ROI = ((Revenue - Budget) / Budget) × 100

ROI is calculated only when valid positive budget and revenue values are available.

📊 Dashboard KPIs

The Power BI dashboard includes the following key performance indicators:

🎬 Total Movies
⭐ Average Rating
💰 Total Revenue
📈 Total Profit
🔄 Average ROI
📈 Dashboard Visualizations

The dashboard provides visual analysis of:

🎭 Genre Analysis
Movies by Genre
Average Rating by Genre
Revenue by Genre
⭐ Rating Analysis
Rating Distribution
Average Rating by Genre
💰 Financial Analysis
Budget vs Revenue
Revenue by Year
Top 10 Movies by Revenue
Top 10 Movies by ROI
📅 Time Analysis
Movies Released by Year
Revenue Trends
🎛️ Interactive Filters

Users can explore the dashboard using filters such as:

Release Year
Rating Category
Original Language

These filters allow users to interactively explore different sections of the movie dataset.

🧮 Power BI Measures

Example DAX measures used in the dashboard:

Total Movies =DISTINCTCOUNT(Movies[id])
Average Rating =AVERAGE(Movies[vote_average])
Total Revenue =SUM(Movies[revenue])
Total Profit =SUM(Movies[profit])
Average ROI =AVERAGE(Movies[roi])
