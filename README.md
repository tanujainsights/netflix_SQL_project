# 🎬 Netflix Data Analysis Using SQL

## 📌 Project Overview

This project analyzes Netflix movies and TV shows using **PostgreSQL and SQL**.

The objective is to explore Netflix's content library, identify important trends, and answer real-world business questions using SQL queries.

The analysis covers content types, ratings, countries, genres, directors, actors, release years, movie duration, and content descriptions.

---

## 🎯 Project Objectives

* Analyze the distribution of Movies and TV Shows
* Identify the most common ratings
* Find countries producing the most Netflix content
* Analyze Netflix content by release year
* Identify the longest movies
* Analyze recently added content
* Find content by specific directors and actors
* Analyze TV shows with multiple seasons
* Identify popular genres
* Analyze India's Netflix content
* Identify movies classified as documentaries
* Find content without directors
* Analyze actors appearing in Indian content
* Categorize content based on keywords in descriptions

---

## 🛠️ Tools & Technologies

* **PostgreSQL**
* **pgAdmin 4**
* **SQL**
* **CSV Dataset**
* **GitHub**

---

## 📂 Dataset

The project uses the **Netflix Titles Dataset**, containing information about Netflix movies and TV shows.

### Important Columns

| Column         | Description                         |
| -------------- | ----------------------------------- |
| `show_id`      | Unique content ID                   |
| `type`         | Movie or TV Show                    |
| `title`        | Title of the content                |
| `director`     | Director of the content             |
| `cast`         | Actors appearing in the content     |
| `country`      | Country where content was produced  |
| `date_added`   | Date added to Netflix               |
| `release_year` | Original release year               |
| `rating`       | Content rating                      |
| `duration`     | Movie duration or number of seasons |
| `listed_in`    | Genre/category                      |
| `description`  | Content description                 |

---

## 🗄️ Database Setup

The dataset was imported into PostgreSQL and stored in a table named:

```sql
netflix
```

Example table creation:

```sql
CREATE TABLE netflix (
    show_id VARCHAR(10),
    type VARCHAR(20),
    title TEXT,
    director TEXT,
    cast TEXT,
    country TEXT,
    date_added VARCHAR(50),
    release_year INT,
    rating VARCHAR(20),
    duration VARCHAR(20),
    listed_in TEXT,
    description TEXT
);
```

---

## 🔍 SQL Analysis

The project contains SQL queries to answer multiple business questions.

### Key Analysis

1. Find the most common rating for Movies and TV Shows
2. List movies released in a specific year
3. Find the top 5 countries with the most Netflix content
4. Identify the longest movie
5. Find content added within the last 5 years
6. Find movies and TV shows by a specific director
7. Find TV shows with more than 5 seasons
8. Count content items by genre
9. Analyze India's content releases
10. Find documentary movies
11. Identify content without a director
12. Analyze movies featuring specific actors
13. Find the top actors appearing in Indian content
14. Categorize content based on keywords in descriptions

---

## 📊 SQL Concepts Used

This project demonstrates practical PostgreSQL skills, including:

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* `HAVING`
* `LIMIT`
* `CASE WHEN`
* `COUNT()`
* `RANK()`
* `STRING_TO_ARRAY()`
* `UNNEST()`
* `SPLIT_PART()`
* `TO_DATE()`
* `ILIKE`
* `EXTRACT()`
* Common Table Expressions (CTEs)
* Window Functions
* Subqueries
* Type Casting
* Data Aggregation

---

## 💡 Key Business Insights

The analysis can be used to identify:

* The proportion of Movies versus TV Shows on Netflix
* The most frequently appearing content ratings
* Countries contributing the highest amount of content
* Popular genres on the platform
* Trends in Netflix content releases
* Longest movies available on the platform
* Growth of Netflix content over time
* Indian content production trends
* Directors and actors with significant representation
* Content with missing director information

---

## 📁 Project Structure

```text
Netflix-Data-Analysis/
│
├── Dataset/
│   └── netflix_titles.csv
│
├── SQL/
│   ├── create_table.sql
│   ├── data_cleaning.sql
│   └── netflix_analysis.sql
│
├── Screenshots/
│   └── query_results.png
│
└── README.md
```

---

## 🚀 How to Run the Project

### 1. Create the database

Create a PostgreSQL database using pgAdmin 4.

### 2. Create the table

Run the table creation SQL script.

### 3. Import the Netflix dataset

Import the CSV file into the `netflix` table using pgAdmin 4's **Import/Export Data** option.

### 4. Verify the data

```sql
SELECT COUNT(*)
FROM netflix;
```

Check sample records:

```sql
SELECT *
FROM netflix
LIMIT 10;
```

### 5. Run the analysis

Open:

```text
SQL/netflix_analysis.sql
```

Run the queries individually or execute the complete script.

---

## 📈 Future Improvements

This project can be extended by:

* Creating a **Power BI Netflix Dashboard**
* Adding more advanced customer/content analysis
* Performing genre-level trend analysis
* Creating time-series visualizations
* Adding additional KPIs
* Combining SQL analysis with Python for deeper exploratory analysis

---

## 👩‍💻 Skills Demonstrated

**SQL | PostgreSQL | Data Analysis | Data Cleaning | Data Exploration | Business Intelligence | Problem Solving | Data Interpretation**

---

## ⭐ Conclusion

This project demonstrates how SQL can be used to transform a raw Netflix dataset into meaningful business insights. It focuses on practical data analysis techniques and real-world business questions that are relevant to a Data Analyst role.
