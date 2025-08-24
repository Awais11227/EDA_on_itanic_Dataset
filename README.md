# 🛳 Titanic Dataset - Exploratory Data Analysis (EDA)

## 📌 Introduction  
This project explores the **Titanic dataset**, one of the most popular datasets for learning data analysis and machine learning. The dataset contains passenger information such as age, gender, class, fare, and survival status.  

The goal of this EDA is to:  
- Understand the dataset structure  
- Identify missing values and data quality issues  
- Explore **univariate** and **bivariate** relationships  
- Engineer new features for better insights  
- Derive conclusions that can be used in predictive modeling  

---

## 📂 Dataset Description  
The dataset contains a mix of **categorical** and **numerical** features:  

### 🔢 Numerical Features  
- `Age` – Age of the passenger  
- `Fare` – Ticket fare  

### 🔤 Categorical Features  
- `Sex` – Gender (male/female)  
- `Embarked` – Port of embarkation (C, Q, S)  
- `Pclass` – Passenger class (1 = Upper, 2 = Middle, 3 = Lower)  
- `Survived` – Survival status (0 = No, 1 = Yes)  

### 🔗 Mixed Features  
- `SibSp` – Number of siblings/spouses aboard  
- `Parch` – Number of parents/children aboard  
- `Ticket` – Ticket number (alphanumeric)  
- `Cabin` – Cabin number (alphanumeric, missing for many)  
- `Name` – Passenger’s name  

---

## 📊 Univariate Analysis  

- **Age**: Right-skewed distribution. Most passengers between 20–40 years.  
- **Fare**: Right-skewed with outliers. Most fares under 50 units.  
- **Sex**: More males than females.  
- **Pclass**: Majority in class 3.  
- **Survived**: 38% survived, 62% did not.  

---

## 🔗 Bivariate Analysis  

- **Survival vs Sex**: Females survived more often than males.  
- **Survival vs Pclass**: Class 1 had higher survival rates than class 3.  
- **Survival vs Age**: Children survived more often than adults.  
- **Correlation Heatmap**: Pclass and Fare strongly related to survival.  

---<img width="533" height="401" alt="image" src="https://github.com/user-attachments/assets/668097be-ea60-4c78-aadc-10065016a91f" />


## 🛠 Feature Engineering  

1. **Family Size** = `SibSp + Parch + 1`  
2. **Individual Fare** = `Fare / (Family Size)`  
3. **Title Extraction** from `Name` (Mr, Mrs, Miss, Master, etc.)  
4. **Surname Extraction** from `Name` (useful for grouping families)  

---

## 📌 Key Insights  
- Women and children had higher survival rates.  
- Passengers in higher classes had better chances of survival.  
- Fare was an important indicator of survival probability.  
- Feature engineering adds more predictive power.  

---
<img width="474" height="331" alt="image" src="https://github.com/user-attachments/assets/dd408e9d-3ee4-4e5f-b8e9-e21d645f8e28" />


