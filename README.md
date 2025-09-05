# Passenger Survival Analytics & Prediction: A Titanic Case Study  

## 📌 Overview  
This project analyzes the Titanic dataset to identify factors affecting passenger survival and builds a predictive model.  
It was developed entirely using *Google Colaboratory (Colab)*, a cloud-based Jupyter notebook environment that integrates easily with GitHub and Google Drive.  

---

## 🔹 Objectives  
- Perform *data cleaning* (handle missing values for Age, Embarked; drop Cabin).  
- Conduct *exploratory data analysis (EDA)* with visualizations.  
- Engineer new features (e.g., Family Size).  
- Build a *Logistic Regression model* to predict survival probability.  
- Derive actionable *insights* (impact of gender, class, and age on survival).  

---

## 🔹 Dataset  
- *Source:* [DatascienceDojo Titanic Dataset](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)  
- *Description:* Includes passenger details such as class, age, gender, family relations, and survival outcome.  

---

## 🔹 Tools & Libraries  
- *Google Colab* (for development & execution)  
- Python libraries:  
  - pandas, numpy → data manipulation  
  - matplotlib, seaborn → visualization  
  - scikit-learn → logistic regression model  

---

## 🔹 Key Steps  
1. *Data Loading & Inspection*  
   - Loaded dataset directly from GitHub raw CSV link.  
   - Checked shape, column details, and missing values.  

2. *Data Cleaning*  
   - Imputed missing Age values with median.  
   - Filled Embarked column with mode.  
   - Dropped Cabin column due to excessive missing values.  

3. *Feature Engineering*  
   - Converted Sex to numeric (male=0, female=1).  
   - Created FamilySize = SibSp + Parch + 1.  

4. *Exploratory Analysis*  
   - Survival rate by Gender, Class, Age distribution, Family Size, Fare.  
   - Used bar plots, box plots, and KDE distributions.  

5. *Modeling*  
   - Logistic Regression with ~78% accuracy.  
   - Evaluated with accuracy score and confusion matrix.  

6. *Insights*  
   - Women and children had higher survival probability.  
   - First-class passengers were prioritized.  
   - Larger families had lower chances compared to small/medium-sized families.  

---

## 🔹 Results (Visual Highlights)  
![Survival Count](outputs/survival_count.png)  
![Survival by Gender](outputs/survival_gender.png)  
![Survival by Class](outputs/survival_class.png)  

---

## 🔹 How to Run  

### 🔸 Run in Google Colab (Recommended)  
Click the link below to open the notebook directly in Colab:  
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Sushmitha-eng/titanic-survival-analytics/blob/main/notebooks/titanic_analysis.ipynb)  

### 🔸 Run Locally (Optional)  
```bash
git clone https://github.com/Sushmitha-eng/titanic-survival-analytics.git
cd titanic-survival-analytics
pip install -r requirements.txt
jupyter notebook notebooks/titanic_analysis.ipynb
