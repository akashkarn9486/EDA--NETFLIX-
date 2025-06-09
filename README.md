
# 📺 Netflix EDA – A Deep Dive into Streaming Trends

### Author: **Akash Karn**

---

## 🧠 Introduction

In the era of digital streaming, **Netflix** has become a household name, producing and distributing a massive volume of content globally. This project undertakes a comprehensive **Exploratory Data Analysis (EDA)** on Netflix's catalog to uncover hidden patterns, understand content distribution across genres, countries, and formats, and reveal consumer-oriented trends.

With Python’s powerful data analysis libraries and compelling visualizations, this project transforms raw data into a story that reveals **how Netflix curates and distributes content to its global audience**.

---

## 📌 Project Objectives

The primary goals of this project are to:

- 📦 Understand the structure and content of the dataset.
- 🔍 Identify trends in the type of content (Movies vs TV Shows).
- 🌍 Analyze geographical content production and distribution.
- 🗓 Explore how Netflix's content library has evolved over time.
- 🎭 Examine the most common genres, durations, and ratings.
- 👨‍💼 Discover popular directors and recurring cast members.
- 📈 Communicate findings using informative and appealing visualizations.

---

## 📁 Dataset Overview

The dataset used in this project includes information on Netflix's titles as of the latest update. It contains the following key features:

| Column Name   | Description                                  |
|---------------|----------------------------------------------|
| `show_id`     | Unique ID for each show                      |
| `type`        | Indicates if it's a Movie or TV Show         |
| `title`       | Title of the content                         |
| `director`    | Director(s) of the content                   |
| `cast`        | Leading actors/actresses                     |
| `country`     | Country of production                        |
| `date_added`  | Date it was added to Netflix                 |
| `release_year`| Original year of release                     |
| `rating`      | Age-based content rating                     |
| `duration`    | Length of the movie or number of seasons     |
| `listed_in`   | Genre categories                             |
| `description` | Short summary of the title                   |

---

## 🧹 Data Cleaning & Preprocessing

A crucial part of this EDA involved data preparation:

- 🧼 **Handling Missing Values**:
  - Fields like `director`, `cast`, and `country` had numerous missing values. Logical imputation or null removal was used contextually.
- 📅 **Date Formatting**:
  - `date_added` was converted into `datetime` format for better temporal analysis.
- 🧭 **Feature Engineering**:
  - Created new columns like `year_added`, `month_added` from `date_added` for seasonal trends.
- 📊 **Categorical Parsing**:
  - The `listed_in` column was tokenized to better analyze genres.

---

## 📊 Visual Insights & Exploratory Analysis

The analysis is richly illustrated with plots created using **Matplotlib** and **Seaborn** to interpret the data visually. Below are some of the key findings:

### 📌 1. Content Type Distribution

A bar chart showing that **Movies constitute ~70%** of the platform's content, indicating a higher production or acquisition rate for movies than TV shows.

---

### 📌 2. Content Added Over the Years

A line graph reveals that **Netflix significantly ramped up content additions from 2016–2019**, peaking in 2019 before dropping slightly in subsequent years.

---

### 📌 3. Country-Wise Content Production

A horizontal bar chart depicts that:

- **USA** dominates in content production.
- **India**, **UK**, and **Canada** are also key contributors.

---

### 📌 4. Genre Analysis

Genres like **Dramas, International Movies, and Comedies** dominate the content library.

- A pie chart illustrates the genre composition.
- Multiple genres per title were handled through tokenization.

---

### 📌 5. Age Rating Distribution

Bar plots show the content rating skew:

- Most content is rated **TV-MA**, suggesting a mature audience focus.
- **TV-14** and **R** also appear frequently.

---

### 📌 6. Duration & Runtime Trends

Duration analysis indicates:

- Most movies are **90–100 minutes** long.
- TV shows with **1 or 2 seasons** are common.

---

### 📌 7. Frequent Directors and Actors

Analyzing director and cast data highlights:

- **Raúl Campos** and **Jan Suter** appear frequently.
- Popular cast members are identified based on recurrence.

---

## 📈 Correlations & Trends

Several multivariate visualizations explore the interplay between `release_year`, `country`, `rating`, and `duration`. These help uncover trends like:

- Increase in **adult-rated** content over the years.
- Growth in **international content** from non-English-speaking countries.
- Rise in content targeting **teenage audiences** post-2015.

---

## 🔧 Tech Stack

| Tool / Library | Purpose                  |
|----------------|--------------------------|
| Python         | Programming Language     |
| Pandas         | Data handling & cleaning |
| Seaborn        | Statistical visualizations |
| Matplotlib     | Plotting & visual design |
| Jupyter Notebook | Interactive analysis     |

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/netflix-eda.git
cd netflix-eda
```

### 2. Install Required Packages
```bash
pip install pandas matplotlib seaborn jupyter
```

### 3. Launch Jupyter Notebook
```bash
jupyter notebook
```

Open the `EDA-Netflix.ipynb` notebook and run all cells to reproduce the analysis.

---

## 🤔 Future Work Ideas

- Sentiment analysis on descriptions using NLP.
- Recommendation system based on genres and durations.
- Compare Netflix content with competitors like Amazon Prime or Disney+.

---

## 🙌 Acknowledgment

Special thanks to the contributors of open Netflix datasets and the data science community for continuous support and inspiration.

---

## 📬 Contact

Feel free to connect or reach out:

**Akash Karn**  
📧 akash.karn.email@gmail.com  
📍 [LinkedIn](https://www.linkedin.com/in/your-profile) | [GitHub](https://github.com/yourusername)
