# 🎬 Netflix Movie Dataset Analysis

**Unlocking insights from Netflix movie data with Python & Jupyter Notebook!**  

_**A comprehensive data cleaning, analysis, and visualization journey.**_

![Alt text](https://github.com/omjaikumar23/Netflix-Data-Analysis/blob/947e4627dde59468c4d7781ffa82f1283823132f/Netflix.jpg)

---

## ✨ Overview

This project analyzes a large Netflix movie dataset using Python (in a **Jupyter Notebook**), applying data wrangling, categorization, and a range of visualizations to uncover insights such as:
- Which genres dominate Netflix’s catalog
- Most and least popular movies and their genres
- Yearly production trends
- Distribution of movie popularity
- And more!

---

## 🔧 Technology Stack & Libraries

- **Jupyter Notebook**: Interactive analysis & visual feedback  
- **Python 3.9.13**
    - `numpy` – Efficient numerics
    - `pandas` – Data handling & transformation
    - `matplotlib` – Core plotting
    - `seaborn` – Advanced statistical visuals

---

## 🗂️ Data Pipeline & Methodology

**Performed in the notebook:**

1. **Data Exploration**
    - Inspect head of data, info, datatypes
    - Summary statistics & duplicate/NaN checks

2. **Data Cleaning & Preparation**
    - 🗓️ Convert `Release_Date` to integer year  
    - 🚮 Drop non-informative columns: `Overview`, `Original_Language`, `Poster_Url`
    - 🏷️ Categorize `Vote_Average` into:  
      `not_popular`, `below_avg`, `average`, `popular` (using quartiles)
    - 🎭 Parse `Genre`:  
      - Split comma-separated genres into lists
      - Explode list into separate rows for genre-level analysis
      - Convert genre to categorical type
    - ✅ Remove duplicates & NaNs

3. **Visualization & Insights**
    - Plot genre frequency, vote categories, trends by year, etc.
    - Highlight most/least popular movies (and genres)
    - Find year with most titles released

---

## 📁 Data Structure After Cleaning

| Column        | Description                                           |
|---------------|-------------------------------------------------------|
| Release_Date  | Year of release (int)                                 |
| Title         | Movie name                                            |
| Popularity    | Numeric popularity score                              |
| Vote_Count    | # of user votes                                       |
| Vote_Average  | Popularity class (`not_popular`, `below_avg`, etc.)   |
| Genre         | Single genre per row (categorical, after explosion)   |

---


_See the full notebook for step-by-step code and results!_

---

## 💡 Insights

- 🎭 **Drama** is the most frequent genre (>14% of titles).
- ⭐ ~25% movies are “popular”—most frequently *Drama*.
- 🕷️ *Spider-Man: No Way Home* leads popularity, spanning Action, Adventure, Sci-Fi.
- 🎼 The lowest popularity: *United States vs. Billie Holiday*, *Threads* (multiple genres).
- 📆 **2020** had the most movie releases in this dataset.

---

## 🚀 Run It Yourself

1. **Clone the repo:**
    ```
    git clone https://github.com/your-username/netflix-movie-analysis.git
    cd netflix-movie-analysis
    ```
2. **Install required packages:**
    ```
    pip install numpy pandas matplotlib seaborn jupyter
    ```
3. **Add the data file:**  
   Place `mymoviesdb.csv` in the project directory.
4. **Start the notebook:**
    ```
    jupyter notebook
    ```
    Open `Netflix_Movie_Analysis.ipynb` and run all cells!

---

## 🤝 Contributions

Feedback, fixes & new ideas welcome via pull requests or issues!

---

## 🙏 Acknowledgments

- Netflix for inspiration & public datasets
- The Python open-source community

---

_Analysis by [Om Jaikumar](https://github.com/omjaikumar23)_  
📝 Built with Jupyter Notebook | 🚀 Happy Exploring!


