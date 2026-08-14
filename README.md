# Diabetes Data Analysis

A comprehensive exploratory data analysis (EDA) on the **Pima Indians Diabetes Dataset** — uncovering patterns, correlations, and insights that drive diabetes prediction.

> *"Data is the new science. Big Data holds the answers."* — Pat Gelsinger

---

## Table of Contents

- [About](#about)
- [Dataset](#dataset)
- [Analysis Highlights](#analysis-highlights)
- [Techniques Used](#techniques-used)
- [Key Insights](#key-insights)
- [How to Run](#how-to-run)
- [Project Structure](#project-structure)
- [Connect](#connect)

---

## About

This project performs a complete exploratory data analysis on diabetes health data. It covers everything from data quality checks to statistical summaries and visualizations — a solid foundation for any machine learning pipeline.

**Tools:** Python, Pandas, Matplotlib, Seaborn  
**Platform:** Google Colab  
**Level:** Beginner → Intermediate Data Analysis

---

## Dataset

The **Pima Indians Diabetes Dataset** contains medical predictor variables for females of Pima Indian heritage aged 21+.

| Feature | Description |
|---------|-------------|
| `Pregnancies` | Number of pregnancies |
| `Glucose` | Plasma glucose concentration (2hr oral glucose tolerance test) |
| `BloodPressure` | Diastolic blood pressure (mm Hg) |
| `SkinThickness` | Triceps skin fold thickness (mm) |
| `Insulin` | 2-Hour serum insulin (mu U/ml) |
| `BMI` | Body mass index (weight in kg/(height in m)²) |
| `DiabetesPedigreeFunction` | Diabetes pedigree function (genetic score) |
| `Age` | Age in years |
| `Outcome` | Diabetes diagnosis (0 = No, 1 = Yes) |

---

## Analysis Highlights

### Data Exploration
- First & last rows inspection
- Dataset shape and dimensions
- Column names and data types
- General info and statistical summary

### Data Quality Checks
- Missing value detection
- Duplicate value identification
- Unique value counts per column
- Invalid zero-value detection (real missing data in medical fields)

### Selection & Filtering
- Single and multi-column selection
- Conditional row filtering (Age > 60, Age > 65 + diabetic)
- Index-based row access with `iloc`

### Sorting & Grouping
- Value counts for outcome distribution
- Group-by operations with aggregation
- Mean, median, and standard deviation calculations
- Full correlation matrix

### Data Modification
- New feature engineering (`BMI_CATEGORY` using `pd.cut`)
- Invalid zero replacement with mean values

### Visualization
- Age distribution histogram
- matplotlib & seaborn plots

---

## Techniques Used

| Technique | Library | Purpose |
|-----------|---------|---------|
| Data Loading | Pandas | Read CSV data |
| Descriptive Statistics | Pandas | `describe()`, `info()`, `mean()`, `median()`, `std()` |
| Missing Data Detection | Pandas | `isnull()`, `duplicated()`, zero-value checks |
| Filtering & Selection | Pandas | Boolean indexing, `iloc`, conditional filters |
| Grouping & Aggregation | Pandas | `groupby()`, `value_counts()`, `corr()` |
| Feature Engineering | Pandas | `pd.cut()` for binning continuous variables |
| Data Cleaning | Pandas | `replace()` for imputation |
| Visualization | Matplotlib, Seaborn | Histograms, distribution plots |

---

## Key Insights

- **Glucose level** is the strongest predictor of diabetes outcome
- **BMI** and **Age** show significant correlation with diabetes presence
- Invalid zero values in `Glucose`, `BloodPressure`, `SkinThickness`, `Insulin`, and `BMI` represent real missing data that needs imputation
- The dataset is **imbalanced** — more non-diabetic cases than diabetic
- Patients over 65 with diabetes have distinctly different health profiles

---

## How to Run

### Option 1: Google Colab (Recommended)
1. Open the notebook in [Google Colab](https://colab.research.google.com/drive/1qotn1cNWxpr0J_NnSbwgvn8fSt4iOHH1)
2. Upload `diabetes.csv` when prompted
3. Run all cells

### Option 2: Local
```bash
# Clone the repo
git clone https://github.com/prabhat8420/Data-analysis.git
cd Data-analysis

# Install dependencies
pip install pandas matplotlib seaborn

# Run the script
python diabities_data_analysis.py
```

> **Note:** Update the CSV path in the script to match your local file location.

---

## Project Structure

```
Data-analysis/
├── README.md
├── LICENSE
├── diabetes.csv                        # Dataset (Pima Indians Diabetes)
└── diabities_data_analysis.py          # Main analysis script
```

---

## Future Scope

- [ ] Add correlation heatmap visualization
- [ ] Build a logistic regression prediction model
- [ ] Create interactive dashboards with Plotly
- [ ] Perform hypothesis testing
- [ ] Add more visualizations (box plots, pair plots)

---

## Connect

**Prabhat** — [GitHub](https://github.com/prabhat8420)

---

<p align="center">
  <i>"Without data, you're just another person with an opinion."</i>
</p>
