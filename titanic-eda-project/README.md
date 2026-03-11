# Titanic Exploratory Data Analysis (EDA)

A complete, portfolio-ready Exploratory Data Analysis project based on the Titanic dataset.

## Project objective

The goal of this project is to explore the Titanic dataset, clean the data, handle missing values, create visualizations, and perform correlation analysis to understand which factors were associated with passenger survival.

## Skills demonstrated

- Data cleaning  
- Missing value handling  
- Exploratory data analysis  
- Data visualization with matplotlib  
- Correlation analysis  
- Feature engineering  
- GitHub-ready project structuring  

## Dataset

This project uses the same column structure and row count as the Kaggle Titanic training dataset (`891` rows, `12` columns).

Original competition page:  
Kaggle Titanic – Machine Learning from Disaster

## Project structure

```bash
titanic-eda-complete/
│
├── data/
│   └── train.csv
├── notebooks/
│   └── Titanic_EDA_Complete.ipynb
├── images/
│   ├── 01_survival_count.png
│   ├── 02_survival_rate_by_sex.png
│   ├── 03_survival_rate_by_class.png
│   ├── 04_age_distribution.png
│   ├── 05_fare_by_class.png
│   └── 06_correlation_matrix.png
├── requirements.txt
└── README.md
```

## Data cleaning and missing value handling

Missing values found in the dataset:

- `Age`: 177 missing values  
- `Cabin`: 687 missing values  
- `Embarked`: 2 missing values  

Cleaning strategy used:

- Filled `Age` with the median value
- Filled `Embarked` with the mode
- Dropped `Cabin` for modeling/correlation because too many values were missing
- Created a new feature called `FamilySize = SibSp + Parch + 1`
- Dropped `PassengerId`, `Name`, and `Ticket` in the encoded dataset used for correlation analysis

## Key findings

- Overall survival rate was **38.4%**
- Female survival rate was **74.2%**
- Male survival rate was **18.9%**
- First-class survival rate was **63.0%**
- Second-class survival rate was **47.3%**
- Third-class survival rate was **24.2%**

## Visualizations included

1. Survival count
2. Survival rate by sex
3. Survival rate by passenger class
4. Age distribution
5. Fare distribution by passenger class
6. Correlation matrix

## How to run

```bash
pip install -r requirements.txt
jupyter notebook
```

Then open:

```bash
notebooks/Titanic_EDA_Complete.ipynb
```

## Portfolio summary

This project is suitable for a beginner data analytics or data science portfolio because it demonstrates a full EDA workflow from raw data inspection to cleaned insights and visual storytelling.

## Suggested GitHub repository name

```bash
titanic-eda-project
```
