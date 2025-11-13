# EDA on Movies Dataset

## 📌 Project Overview

This project performs an in-depth **Exploratory Data Analysis (EDA)** on a Movies dataset containing **9,827 movie records** across **9 features**. The analysis covers data cleaning, preprocessing, transformation, visualization, and insight extraction. The goal is to understand trends in movie genres, languages, ratings, popularity, and release patterns.

---

## 📂 Dataset Description

**Total Rows:** 9,827
**Total Columns:** 9

### **Columns Used**

* **Release_Date** – Movie release year
* **Title** – Movie title
* **Overview** – Movie description
* **Popularity** – Popularity score
* **Vote_Count** – Number of votes
* **Vote_Average** – Average rating
* **Original_Language** – Language ISO code
* **Genre** – Genre list
* **Poster_Url** – Poster link

The dataset required cleaning and restructuring before analysis, including:

* Removing unused columns
* Splitting/Exploding multi-genre columns
* Handling categorical data
* Converting language ISO codes to full names

---

## 🧹 Data Cleaning & Preprocessing

Key steps performed:

* Removed unnecessary columns
* Converted ISO language codes → Full language names
* Split `Genre` column into lists and used `explode()` for analysis
* Converted `Genre` into `category` dtype for memory efficiency
* Verified duplicates and missing values (none found)
* Standardized column types

---

## 📊 Key Insights

### **1️⃣ Genre Distribution**

After exploding the Genre column:

* Total genres identified: **19**
* **Top 5 Genres (by count):**

  * Drama — **3,610 movies (14.5%)**
  * Comedy — **2,975 movies (11.9%)**
  * Action — **2,600 movies (10.4%)**
  * Thriller — **2,368 movies (9.5%)**
  * Adventure — **1,790 movies (7.2%)**
* These top 5 genres account for **53.5%** of all movies.
* Remaining genres combined into **"Other"** category — **46.5%**.

---

### **2️⃣ Language Insights**

* The dataset contains movies in **40+ unique languages**.
* **English movies dominate (~70%)**, making it the primary language of production.
* Major non‑English contributors: French, Japanese, Hindi, and Spanish.
* Non-English films still show strong ratings and popularity.

---

### **3️⃣ Release Year Trends**

* Movies range from **1902 to 2022**.
* Sharp increase in production post‑1980.
* Peak production years: **2018–2021 (~15% of all movies)**.
* The highest single-year output was around **2019**.

---

### **4️⃣ Ratings & Popularity**

* Average rating (Vote_Average): **6.5–7.0** range.

#### **Top 5 Highest-Rated & Most Popular Movies (One per Language)**

1. **Spider‑Man: No Way Home (2021, English)** — 8.3 rating | 5083.9 popularity
2. **Capernaum (2018, Arabic)** — 8.2 rating | 21.1 popularity
3. **Winter on Fire (2015, Ukrainian)** — 8.0 rating | 25.2 popularity
4. **Children of Heaven (1997, Persian)** — 7.9 rating | 26.0 popularity
5. **Through My Window (2022, Spanish)** — 7.8 rating | 659.1 popularity

These represent top-performing films across multiple languages, showing diverse cinematic excellence.

---

## 🧠 Key Takeaways

* Dataset is **clean and analysis-ready** — no missing or duplicate values.
* Genre distribution shows clear dominance of **Drama and Comedy**.
* English dominates production volume, but non-English films excel in ratings.
* Post‑1980 global movie production shows exponential growth.
* Highest-rated films come from a **mix of global regions**, not just English.

---

## 📌 Tools & Libraries Used

* **Python**
* **Pandas** (data cleaning & manipulation)
* **Matplotlib** & **Seaborn** (visualization)
* **NumPy**
* **Jupyter Notebook**

---

## 🚀 How to Run the Notebook

1. Clone the repository:

```bash
git clone https://github.com/PranayDomal/EDA_Movies_Dataset.git
```

2. Navigate to the folder:

```bash
cd EDA_Movies_Dataset
```

3. Install dependencies:

```bash
pip install -r requirements.txt
```

4. Run the notebook:

```bash
jupyter notebook EDA_Movies_Dataset.ipynb
```

---

## 📎 Project Structure

```
├── EDA_Movies_Dataset.ipynb
├── mymoviedb.csv
├── README.md
├── requirements.txt
```

---

## 📄 License

This project is released under the **MIT License**.
