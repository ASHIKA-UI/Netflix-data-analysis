# Netflix Data Analysis using Python

## 📌 Project Overview

This project performs **Exploratory Data Analysis (EDA)** on the Netflix Movies and TV Shows dataset to understand content trends, popular genres, production countries, and content growth over the years.

The analysis was performed using **Python, Pandas, Matplotlib, and Seaborn**.
The goal of the project is to extract **meaningful insights from the dataset and visualize them using graphs**.

---

## 📂 Dataset

The dataset used in this project is **Netflix Movies and TV Shows Dataset**, which contains information about Netflix content including:

* Show ID
* Title
* Type (Movie or TV Show)
* Director
* Cast
* Country
* Date Added
* Release Year
* Rating
* Duration
* Genre
* Description

Dataset size: **8800+ records**

---

## 🛠 Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook / VS Code

---

## 📊 Key Analysis Performed

### 1️⃣ Movies vs TV Shows

Analyzed the distribution of Movies and TV Shows available on Netflix.

### 2️⃣ Netflix Content Growth Over the Years

Analyzed how Netflix content increased over time based on the **date_added** column.

### 3️⃣ Top Countries Producing Netflix Content

Identified which countries produce the most Netflix content.

### 4️⃣ Popular Genres

Analyzed the most common genres available on Netflix.

### 5️⃣ Top Directors

Identified directors with the highest number of titles on Netflix.

### 6️⃣ Movie Duration Analysis

Studied the distribution and average duration of Netflix movies.

---

## 🧹 Data Cleaning

Before performing analysis, the dataset required preprocessing:

* Removed leading spaces in **date_added**
* Converted **date_added** to datetime format
* Extracted **year_added** from the date
* Handled missing values in columns such as **country** and **director**

Example:

```python
data['date_added'] = data['date_added'].str.strip()
data['date_added'] = pd.to_datetime(data['date_added'], errors='coerce')
data['year_added'] = data['date_added'].dt.year
```

---

## 📈 Visualizations

The project includes several visualizations:

* Bar charts
* Line charts
* Histogram
* Count plots

These visualizations help understand trends and patterns in Netflix content.

---

## 🔍 Key Insights

Some insights obtained from the analysis include:

* Netflix contains **more movies than TV shows**
* Content production increased significantly after **2016**
* **United States and India** produce the most Netflix titles
* **Drama and International content** are among the most popular genres
* Average Netflix movie duration is around **90–110 minutes**

---

## ▶ How to Run the Project

1. Install required libraries

```
pip install pandas numpy matplotlib seaborn
```

2. Run the analysis script

```
python netflix_analysis.py
```

3. The program will display:

* dataset preview
* analysis results
* visualizations

---

## 📁 Project Structure

```
Netflix-Data-Analysis
│
├── netflix_titles.csv
├── netflix_analysis.py
└── README.md
```

---

## 🎯 Learning Outcomes

Through this project, the following data analytics skills were developed:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Data Visualization
* Feature Engineering
* Insight Generation

---

## 🚀 Future Improvements

Possible enhancements to this project include:

* Building an **interactive dashboard**
* Creating a **Netflix recommendation system**
* Using **machine learning to predict content trends**

---

## 👩‍💻 Author

Ashika B

This project was created as part of a **Data Analytics portfolio project** to demonstrate practical data analysis skills using Python.
