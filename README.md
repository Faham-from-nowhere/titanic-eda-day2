# Task 2: Exploratory Data Analysis (EDA) – Titanic Dataset

## 🎯 Objective
Perform visual and statistical EDA to understand the Titanic dataset and extract meaningful patterns that could be useful for predictive modeling.

## 🛠️ Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
- Plotly

## 📁 Dataset
- Source: [Kaggle – Titanic: Machine Learning from Disaster](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- File used: `train.csv`

## 📌 Key Operations Performed
- Summary statistics for numeric and categorical columns
- Null value and outlier detection
- Feature engineering:
  - Title extraction from name
  - Family size and is-alone flag
  - Fare per person
  - Age binning
- Visualizations:
  - Histograms, boxplots, countplots, pairplots
  - Correlation heatmap


## 📊 Key Insights from Exploratory Data Analysis (EDA)

- **Age Distribution**: The age range of passengers is wide, with most being between 20 and 40. There are a few senior passengers and a small number of infants.

- **Fare Distribution**: Skewed to the right; most fares are low, but a few passengers paid extremely high fares (upper-class).

- **Survival Rate**:
  - Females had a significantly higher survival rate than males.
  - Passengers in **1st class** had the highest survival rate.
  - **Alone passengers** were less likely to survive.

- **Title Feature**: Titles extracted from names (`Mr`, `Mrs`, `Miss`, etc.) show strong patterns. Some rare titles like `Sir`, `Lady`, and `Countess` were found in first class.

- **Family Size**:
  - Small families (2-4 people) had higher survival chances.
  - Solo travelers and large families had lower survival rates.

- **Correlation Heatmap**:
  - `Fare` and `Pclass` are moderately negatively correlated.
  - `Survived` correlates positively with `Fare` and negatively with `Pclass`.

- **Outliers**: Detected in `Fare`, especially for high-paying passengers. Boxplots helped visualize these extreme values.

- **Pairplot**: Clearly shows clustering patterns for survival based on `Fare`, `Age`, and `Pclass`.



## 💾 Files Included
- `titanic_eda.ipynb`: Jupyter Notebook with all EDA steps
- `Titanic-Dataset.csv`: Dataset used
- `README.md`: This file
