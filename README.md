# 🧠 Employee Attrition & Financial Impact Analysis

This machine learning project combines **classification** and **regression** to help companies:
- Predict which employees are likely to leave
- Estimate future salary of those who stay
- Calculate the expected financial loss from attrition

📌 Built using: Python, Scikit-learn, Pandas, Matplotlib, Seaborn  
📁 Dataset: IBM HR Analytics Attrition Dataset [(https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset]

---

## 📌 Objectives

1. **Attrition Prediction** (Classification)
2. **Future Salary Simulation** (based on performance)
3. **Future Salary Prediction** (Regression)
4. **Identify Employees Likely to Stay**
5. **Estimate Expected Financial Loss**

---

## 📈 Key Results

### 🎯 Classification (Logistic Regression)
- **F1 Score**: 0.448
- **AUC-ROC**: 0.772
- **Precision**: 0.684
- **Recall**: 0.333
- **Cross-Validation F1 Score**: 0.4639

### 💵 Regression (Future Salary)
- **Best Model**: Lasso Regression  
- **R² Score**: 0.9997  
- **RMSE**: 88.13

| Model          | R² Score | RMSE    |
|----------------|----------|---------|
| Random Forest  | 0.9993   | 134.25  |
| Ridge          | 0.9997   | 88.41   |
| **Lasso**      | **0.9997** | **88.13** |
| SVR            | -0.1056  | 5304.15 |

### 📉 Financial Impact
- **Total Expected Loss**: `$1,234,568.92`  
  Formula:  
  `ExpectedLoss = P(Attrition) × FutureSalary`

---

## 📊 Visualizations Included

✔️ Attrition distribution  
✔️ ROC Curve for classifier  
✔️ Salary distribution (before vs simulated)  
✔️ Top 10 feature importances (Random Forest)  
✔️ Expected loss distribution across employees




## ▶️ How to Run This Project

1. Open [Google Colab](https://colab.research.google.com)
2. Upload the file: `Employee_Attrition_Analysis_Colab_Visual.ipynb`
3. Upload the dataset file: `WA_Fn-UseC_-HR-Employee-Attrition.csv`
4. Run each cell step-by-step to see models, outputs, and plots

---

## 💡 Future Work Suggestions

- Use SHAP or LIME for model explainability  
- Add additional features like bonus history or project load  
- Try ensemble stacking (Random Forest + Ridge etc.)  
- Extend analysis to include time-based churn trends

