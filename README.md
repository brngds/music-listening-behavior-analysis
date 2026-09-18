# 🎵 Music Streaming Behavior Analysis

Exploratory data analysis of music streaming behavior in two cities using **Python** and **Pandas**, with a focus on data cleaning, user activity patterns, and hypothesis evaluation.

## 📌 Context

Understanding how users interact with a digital product can help companies identify behavioral patterns and support better data-driven decisions.

In this project, data from a music streaming service was analyzed to compare listening activity between users from **Springfield** and **Shelbyville** across different days of the week.

The project was developed as part of my Data Science studies and focuses on applying fundamental data analysis techniques to a real-world-style dataset.

## 🎯 Problem

The main objective was to investigate whether music streaming activity differs depending on the **city** and **day of the week**.

The hypothesis evaluated was:

> **User activity differs depending on the day of the week and the city.**

To investigate this hypothesis, the dataset first needed to be explored and cleaned before comparing user activity patterns.

## 📊 Dataset

The original dataset contains **65,079 music streaming records** with the following information:

* `user_id` — unique user identifier
* `track` — track title
* `artist` — artist name
* `genre` — music genre
* `city` — user's city
* `time` — time when the track was played
* `day` — day of the week

The analysis focuses on activity recorded on **Monday, Wednesday, and Friday**.

## 💡 Approach

The analysis was divided into three main stages:

### 1. Data Exploration

The dataset was inspected to understand:

* dataset dimensions;
* column structure;
* data types;
* missing values;
* duplicate records;
* categorical inconsistencies.

### 2. Data Cleaning

The preprocessing stage included:

* standardizing column names;
* handling missing values;
* removing duplicate records;
* standardizing inconsistent music genre labels.

A total of **3,826 duplicate records** were identified and removed.

After preprocessing, the dataset contained **61,253 records**.

### 3. Behavioral Analysis

User activity was compared across cities and days of the week to identify differences in listening patterns.

The number of music plays was aggregated for each combination of city and day.

## 🔎 Analysis & Solution

The comparison produced the following activity levels:

| Day       | Springfield | Shelbyville |
| --------- | ----------: | ----------: |
| Monday    |      15,740 |       5,614 |
| Wednesday |      11,056 |       7,003 |
| Friday    |      15,945 |       5,895 |

The results reveal different activity patterns between the two cities.

In **Springfield**, activity is higher on Monday and Friday, with Friday presenting the highest number of plays.

In **Shelbyville**, the highest activity occurs on Wednesday.

Springfield also has a substantially higher absolute number of plays in the dataset. However, this should not automatically be interpreted as greater engagement per user because the analysis does not control for differences in the number of users represented in each city.

## 📈 Key Findings

The analysis identified three main patterns:

* Springfield shows higher absolute streaming activity across all analyzed days.
* Springfield's activity is concentrated primarily on Monday and Friday.
* Shelbyville presents a different pattern, with its highest activity occurring on Wednesday.

Therefore, the observed data is **consistent with the hypothesis that streaming activity varies according to both city and day of the week**.

## 💼 Potential Business Applications

Although this is an exploratory project, similar behavioral analyses could support decisions such as:

* identifying periods of higher user engagement;
* optimizing the timing of marketing campaigns and notifications;
* adapting content recommendations based on behavioral patterns;
* identifying differences in engagement between geographic segments.

These applications would require additional analysis and validation before being used for business decisions.

## 🛠️ Technologies Used

* Python
* Pandas
* Jupyter Notebook
* Exploratory Data Analysis (EDA)
* Data Cleaning
* Data Aggregation

## 📚 Key Learnings

This project helped strengthen fundamental data analysis skills, including:

* exploring unfamiliar datasets;
* identifying data quality issues;
* handling missing and duplicated data;
* standardizing categorical variables;
* grouping and filtering data with Pandas;
* comparing behavioral patterns between groups;
* interpreting analytical results while considering dataset limitations.

One important takeaway was the importance of distinguishing between **patterns observed in a dataset** and conclusions that can be generalized to an entire population.

## ⚠️ Limitations

This analysis is descriptive and does not include an inferential statistical hypothesis test with a significance level or p-value.

The results therefore describe patterns present in the available dataset and should not be interpreted as statistical proof of differences across the entire populations of Springfield and Shelbyville.

Additionally, differences in the number of users represented in each city may influence absolute activity levels.

## 📂 Repository Structure

```text
music-listening-behavior-analysis/
│
├── README.md
│
├── data/
│   └── music_project_en.csv
│
└── notebook/
    └── music_streaming_analysis.ipynb
```

## ▶️ Running the Project

Clone the repository and open the Jupyter Notebook located in the `notebook` directory.

The dataset used by the notebook is stored in the `data` directory.

The analysis requires Python and Pandas.

---

### Author

**Brunno Almeida**

Data Science | Data Analytics | Python | SQL | Machine Learning
