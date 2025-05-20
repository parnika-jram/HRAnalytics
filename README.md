# IBM HR Analytics Employee Attrition & Performance

This project analyzes the **IBM HR Analytics Employee Attrition & Performance** dataset to identify key factors driving employee attrition and to build predictive models.

## 📁 Dataset
- **Source:** IBM Watson's Dataset available on Kaggle: https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
- **Records:** 1,470 employees
- **Features:** 35 columns (e.g., Age, Department, JobSatisfaction, Attrition, etc.)

---

## 🎯 Objectives

1. Identify key factors influencing employee attrition.
2. Test whether job satisfaction significantly differs between employees who leave and those who stay.
3. Predict attrition using features such as job role, salary, and work-life balance.
4. Examine whether longer working hours increase attrition risk.
5. Determine the most important features for predicting attrition.

---

## 🧹 Step 1: Data Cleaning

- Removed irrelevant columns: `EmployeeNumber`, `Over18`, `EmployeeCount`, `StandardHours`
- Converted `Attrition` to binary (Yes → 1, No → 0)
- Encoded categorical variables using One-Hot Encoding

---

## 📊 Step 2: Data Summarization

- Descriptive statistics for numerical features
- Attrition rate calculation
- Mean comparisons by attrition status (e.g., income, satisfaction)

---

## 📈 Step 3: Visualization

- Countplot: Attrition by Job Role
- Boxplots: Monthly Income and Job Satisfaction by Attrition
- Correlation heatmap of numerical and encoded features

---

## 🔗 Step 4: Correlation Analysis

- Computed Pearson correlation between features and `Attrition`
- Identified high-risk factors such as `OverTime`, `JobRole`, `MonthlyIncome`, and `WorkLifeBalance`

---

## 📐 Step 5: Hypothesis Testing

- **T-Test:** Compared `JobSatisfaction` between employees who left and those who stayed
- **OverTime Analysis:** Evaluated the proportion of attrition among employees working overtime

---

## 🤖 Step 6: Machine Learning

- **Models Used:** Random Forest Classifier
- **Steps:**
  - Train/test split with stratification
  - Model training and prediction
  - Evaluation using classification report and confusion matrix
- **Top Predictive Features:**
  - `OverTime`
  - `MonthlyIncome`
  - `JobRole`
  - `Age`
  - `WorkLifeBalance`

---

## 🧠 Insights

- Employees working overtime are significantly more likely to leave.
- Job satisfaction is moderately lower among employees who leave.
- Work-life balance, income, and role are strong predictors of attrition.

---

## 📦 Dependencies

- Python 3.8+
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn
- scipy

---

## 🚀 How to Run

1. Clone the repository.
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
