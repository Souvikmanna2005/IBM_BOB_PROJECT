# 🎬 Netflix Titles — Data Analytics & AI Project

> **IBM SkillsBuild Data Analytics with AI Internship**  
> **Author:** Souvik Manna

---

## 📋 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** and applies **AI / Machine Learning** techniques on the [Netflix Titles dataset](https://www.kaggle.com/datasets/shivamb/netflix-shows) (8,807 titles). The goal is to uncover meaningful insights about Netflix's content library and demonstrate end-to-end data analytics skills.

---

## 📁 Project Structure

```
IBM_Project_Souvik/
│
├── netflix_titles.csv                             # Source dataset
├── SouvikMannaNetflix Data Analytics Project.ipynb  # Main Jupyter Notebook
├── requirements.txt                               # Python dependencies
├── README.md                                      # Project documentation
└── SouvikMannaProjectReport.docx                  # Professional project report
```

---

## 🔍 What's Inside the Notebook

| Section | Description |
|---------|-------------|
| **Step 1** | Import all required libraries |
| **Step 2** | Load & Inspect the Dataset |
| **Step 3** | Data Cleaning & Preprocessing |
| **Step 4** | Exploratory Data Analysis (10 charts) |
| **Step 5** | NLP — Word Cloud from descriptions & genres |
| **Step 6** | AI/ML — Content-Type Classifier (Logistic Regression + Naïve Bayes) |
| **Step 7** | Insights, Findings & Recommendations |

---

## 📊 Key Analyses & Visualizations

- **Content Type Distribution** — Movies vs TV Shows (Bar + Pie)
- **Content Added Over Years** — Grouped bar by year
- **Top 15 Countries** by content count
- **Rating Distribution** — All age ratings visualized
- **Top 15 Genres** — Exploded from the `listed_in` column
- **Movie Duration Analysis** — Histogram + Box Plot
- **TV Show Seasons Distribution** — Bar chart
- **Top 10 Directors** — Most prolific on Netflix
- **Release Year Trend** — Line chart 1990–2021
- **Country × Genre Heatmap** — Cross-tabulation
- **Word Clouds** — Description text & Genre tags
- **ML Confusion Matrices** — Side-by-side model comparison
- **TF-IDF Feature Importance** — Top keywords per class

---

## 🤖 AI / Machine Learning

### Task
Classify Netflix titles as **Movie** or **TV Show** using only the **description** text.

### Pipeline
1. TF-IDF Vectorization (`max_features=5000`, unigrams + bigrams)
2. Train/Test split — 80/20 with stratification
3. Two classifiers trained and compared:
   - **Logistic Regression**
   - **Multinomial Naïve Bayes**

### Results

| Model | Accuracy |
|-------|----------|
| Logistic Regression | ~76% |
| Multinomial Naïve Bayes | ~74% |

---

## 📈 Key Insights

1. **~69.6% Movies** — Netflix is predominantly a movie platform
2. **Content peaked 2018–2019** — Significant growth before COVID-19
3. **USA leads** with 2,818 titles; India follows with 972
4. **TV-MA is #1 rating** — Mature content dominates
5. **Dramas & Comedies** are the most common genres globally
6. **Average movie = ~99 minutes** (median: 98 min)
7. **Most TV shows have 1 season** — Short-run content is popular
8. **Text-based AI** can classify content type with ~76% accuracy

---

## 🛠️ Setup & Installation

### Prerequisites
- Python 3.8+
- pip or conda

### Installation

```bash
# Clone the repository / navigate to project folder
cd IBM_Project_Souvik

# Install dependencies
pip install -r requirements.txt

# Launch Jupyter Notebook
jupyter notebook "SouvikMannaNetflix Data Analytics Project.ipynb"
```

---

## 📦 Dependencies

| Library | Purpose |
|---------|---------|
| `pandas` | Data loading & manipulation |
| `numpy` | Numerical computation |
| `matplotlib` | Core plotting |
| `seaborn` | Statistical visualizations |
| `scikit-learn` | Machine learning (TF-IDF, LR, NB, metrics) |
| `wordcloud` | Word cloud generation |
| `jupyter` | Interactive notebook environment |

---

## 📝 Dataset

| Property | Value |
|----------|-------|
| **Source** | [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows) |
| **Rows** | 8,807 |
| **Columns** | 12 |
| **Key Columns** | `type`, `title`, `director`, `cast`, `country`, `date_added`, `release_year`, `rating`, `duration`, `listed_in`, `description` |

---

## 🎓 About

This project was developed as part of the **IBM SkillsBuild Data Analytics with AI Internship**. It demonstrates practical skills in:
- Data wrangling and preprocessing
- Exploratory data analysis
- Data storytelling through visualization
- Natural Language Processing (NLP)
- Machine Learning classification

---

*Made with ❤️ by Souvik Manna | IBM SkillsBuild Internship*
