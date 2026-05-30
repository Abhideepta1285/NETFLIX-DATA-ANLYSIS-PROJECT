# 🎬 Netflix Movies Data Analysis Project

## 📌 Project Overview

This project focuses on analyzing Netflix movie data using **Python, Pandas, NumPy, Matplotlib, and Seaborn**. The main objective is to clean, preprocess, explore, and visualize the dataset to discover meaningful insights about movies available on Netflix.

---

## 📂 Dataset Information

- **Rows:** 9,827
- **Columns:** 9

The dataset contains information about Netflix movies such as:

- Title
- Genre
- Release Date
- Popularity
- Vote Average
- Vote Count
- And other movie-related attributes

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

### 1. Dataset Inspection
- Checked dataset shape and structure.
- Verified data types of all columns.
- Explored summary statistics.

### 2. Missing Values & Duplicates
- No missing values (NaN) found.
- No duplicate records found.

### 3. Date Formatting
- Converted the `Release_Date` column into datetime format.
- Extracted only the release year for easier analysis.

### 4. Dropping Unnecessary Columns
The following columns were removed because they were not required for analysis:

- `Overview`
- `Original_Language`
- `Poster_Url`

### 5. Vote Average Categorization
The `Vote_Average` column was categorized into four groups:

| Vote Average Category | Description |
|----------------------|-------------|
| Popular | High-rated movies |
| Average | Moderately rated movies |
| Below Average | Below average ratings |
| Not Popular | Low-rated movies |

A custom function `categorize_col()` was used to perform this categorization.

### 6. Genre Processing
- Split multiple genres into individual genres.
- Removed extra whitespaces.
- Used dataframe explosion to create one genre per row.

This allowed more accurate genre-based analysis.

---

## 📊 Exploratory Data Analysis (EDA)

After preprocessing, several business and analytical questions were explored.

### 1️⃣ What is the most frequent genre on Netflix?

- Identified the genre that appears most frequently in the dataset.
- Visualized genre distribution using charts.

### 2️⃣ Which movie has the highest vote average?

- Found the movie with the highest rating based on the `Vote_Average` column.

### 3️⃣ Which movie has the highest popularity?

- Identified the most popular movie in the dataset.
- Examined its associated genre.

### 4️⃣ Which movie has the lowest popularity?

- Found the least popular movie.
- Analyzed its genre category.

### 5️⃣ Which year had the highest number of movie releases?

- Counted movie releases by year.
- Identified the year with the maximum number of movies released.

---

## 📈 Visualizations

The project includes visualizations such as:

- Genre Distribution Charts
- Popularity Analysis
- Vote Average Analysis
- Movie Release Trend by Year
- Highest & Lowest Popularity Comparisons

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📁 Project Structure

```
NETFLIX DATA ANALYSIS PROJECT/
│
├── NETFLIX DATA ANALYSIS.ipynb
├── mymoviesdb.csv
├── README.md
└── images/
    ├── genre_distribution.png
    ├── movies_by_year.png
    └── Vote distribution.png


---

## 🔍 Key Insights

- The dataset contains **9,827 movies**.
- No missing values or duplicate records were found.
- Genre-wise analysis reveals the most dominant movie categories on Netflix.
- Popularity and vote-based metrics help identify top-performing movies.
- Release year trends show periods of increased movie production.

---


## 🎯 Learning Outcomes

Through this project, I practiced:

- Data Cleaning
- Data Preprocessing
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Extracting Business Insights using Python

---

## 👨‍💻 Author

**Abhideepta**

MCA Student | Aspiring Data Scientist | Machine Learning & Generative AI Enthusiast

---

⭐ If you found this project useful, consider giving it a star on GitHub.