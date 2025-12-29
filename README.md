# 🤖 AI Impact on Jobs 2030 – Exploratory Data Analysis & Modeling

## 📌 Project Overview
This project explores the potential impact of **Artificial Intelligence (AI)** on jobs by the year **2030**. Using a structured dataset from Kaggle, the goal was to understand job-related factors associated with automation risk and evaluate whether these factors can reliably predict automation outcomes.

Rather than focusing only on prediction, this project emphasizes **exploration, interpretation, and modeling limits**, which reflects real-world data science practice.

---

## 📊 Dataset Summary
- **Source:** Kaggle – *[AI Impact on Jobs 2030](https://www.kaggle.com/datasets/khushikyad001/ai-impact-on-jobs-2030/data)*
- **Size:** 3,000 rows × 18 columns
- **Key Features:**
  - 💼 Job Title
  - 💰 Average Salary
  - ⏳ Years of Experience
  - 🎓 Education Level
  - 🤖 AI Exposure Index
  - 📈 Tech Growth Factor
  - ⚠️ Automation Probability (2030)
  - 🏷️ Risk Category (Low / Medium / High)

✔️ No missing values  
✔️ Correct data types  
✔️ No data cleaning required  

---

## 🔍 Exploratory Data Analysis (EDA)
Key observations from EDA include:

- 📉 **Automation Probability** is mostly centered between **0.35 – 0.6**
- 🤖 **AI Exposure Index** clusters around mid values, with a few highly exposed jobs
- ⚠️ **Risk Category** is dominated by *Medium* risk
- 🎓 Education levels show **very similar automation risk**
- 🔗 Correlation analysis shows **weak relationships** between features
- 📊 Scatter plots reveal no clear linear trends

These results suggest **heavy overlap** between groups and weak separability.

---

## 🧠 Modeling Approach
To fully assess the problem, multiple models were tested — from simple to advanced.

### 🔹 Classification Models (Risk Category)
- Logistic Regression
- Decision Tree Classifier  

📉 Result:  
Models strongly favored the *Medium* class and failed to distinguish *High* and *Low* risk effectively.

---

### 🔹 Regression Models (Automation Probability)
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor  

📉 Results:
- **MAE ≈ 0.21–0.22**
- **R² ≈ 0 or negative across all models**

Even advanced models failed to outperform a baseline prediction.

---

## 🌳 Feature Importance Insights
Across tree-based models, the most influential features were:

1. 💰 Average Salary  
2. 🤖 AI Exposure Index  
3. 📈 Tech Growth Factor  
4. ⏳ Years of Experience  
5. 🎓 Education Level (minimal impact)

This suggests that **education alone does not strongly protect against automation**, while AI exposure and economic factors play a larger role.

---

## 🧩 Key Takeaways
- ❌ The dataset does **not support reliable prediction** of automation risk
- 📉 Weak feature–target relationships lead to poor model performance
- 🧠 The target variable may be **synthetic or weakly constructed**
- ✅ Identifying modeling limits is a **valid and valuable outcome**

> Sometimes the most important insight is knowing **when a problem cannot be solved with the given data**.

---

## 🚀 Tools & Technologies
- Python 🐍
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn
- Google Colab

---

## 📌 Conclusion
This project demonstrates a **complete data science workflow**:
- Thoughtful exploration
- Appropriate model selection
- Proper evaluation
- Honest interpretation

Rather than forcing conclusions, the analysis highlights the **limitations of the data**, which is a critical skill in real-world analytics and machine learning projects.

---

📁 *For full analysis and code, see the Jupyter Notebook in this repository.*
