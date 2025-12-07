# 📊 Customer Churn Prediction Using Machine Learning

This project predicts **customer churn** using machine-learning models such as  
**Logistic Regression, Random Forest, Decision Tree, and XGBoost**.  
The final optimized model achieves **81.8% recall** and **0.847 ROC-AUC**,  
which makes it highly effective for identifying customers who are likely to leave.

---

## 🚀 Project Overview
Customer churn is one of the most common business problems in telecom, finance, and subscription services.  
The goal of this project is to build a model that:

- Predicts which customers are likely to churn  
- Maximizes **recall** (catch as many churners as possible)  
- Produces interpretable and actionable insights  
- Can be deployed into a real business pipeline  

---

## 📁 Dataset Information
The dataset includes:

- Tenure, Monthly Charges, Total Charges  
- Contract Type  
- Payment Method  
- Internet & Phone Services  
- Demographic Information  
- Target Column: **Churn (Yes/No)**

---

## 🛠️ Data Preprocessing

✔ Handled missing values  
✔ Converted `TotalCharges` into numeric  
✔ Created engineered feature `ChargesPerMonth`  
✔ One-Hot Encoded categorical variables  
✔ Standard-scaled numerical columns  
✔ Train-test split (80/20)  
✔ Checked class balance (SMOTE **not needed** because data was already balanced)

---

## 🤖 Models Trained

| Model | Why Used |
|-------|----------|
| Logistic Regression | Interpretable, stable, great baseline |
| Random Forest | Non-linear patterns |
| Decision Tree | Simple, good for understanding splits |
| XGBoost | Powerful boosting algorithm |

---

## 🧪 Model Performance (Final Tuned Model)

| Metric | Score |
|--------|--------|
| **Accuracy** | 0.724 |
| **Precision** | 0.489 |
| **Recall** | **0.818** |
| **F1 Score** | 0.612 |
| **ROC-AUC** | **0.847** |

➡️ **Recall (81.8%) and AUC (0.847) are excellent** for churn prediction,  
because the primary business goal is to **catch as many churners as possible**.

---

## 🏆 Final Best Model: Logistic Regression (with class weight balancing)

### Why?
- Highest **AUC**  
- Highest **Recall**  
- Easier to deploy & interpret  
- More stable than tree-based models  

---

## 📉 Evaluation Plots
- Confusion Matrix  
<img width="513" height="457" alt="image" src="https://github.com/user-attachments/assets/ba5489bb-b7e2-420a-93bb-cabce50f51ab" />
- ROC Curve
- <img width="464" height="469" alt="image" src="https://github.com/user-attachments/assets/280b18c0-7d1a-4713-9db6-a86894860c56" />
---

## 📌 Future Improvements
- Add model explainability using SHAP  
- Try CatBoost & LightGBM  
- Deploy model using FastAPI / Flask  
- Build a dashboard with Streamlit  
