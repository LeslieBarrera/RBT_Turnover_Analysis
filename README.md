# 🧠 RBT Turnover & Retention Analysis

## **📌 Project Overview**
This project explores **RBT (Registered Behavior Technician) turnover trends** and uses **AI-driven models** to predict retention risks. By analyzing work conditions, supervision feedback, burnout, and other factors, we aim to help **ABA clinics improve employee retention** through **data-driven decision-making**.

## **🎯 Problem Statement**
High **turnover rates** in ABA therapy can disrupt client care, increase training costs, and reduce workforce stability. However:
- **Retention insights are not actively tracked** in most ABA organizations.
- **RBT burnout, supervision quality, and work-life balance** impact retention.
- **AI-based predictive modeling** can **flag at-risk employees early** for intervention.

## **🚀 Solution**
✅ **Analyze RBT data** to identify factors influencing turnover.  
✅ **Develop AI models** to predict which RBTs are at risk of leaving.  
✅ **Compare different machine learning models** for the most effective predictions.  
✅ **Provide actionable insights** for ABA supervisors to improve RBT retention.  

---

## **🔍 Data & Methodology**
### **📊 Data Overview**
We generated a **synthetic dataset** containing **900 RBT records**, including:
- **Demographics & Experience:** Age, education level, years in the field.
- **Work Conditions:** Caseload, hours worked, hourly wage.
- **Supervision Feedback:** BCBA communication, goal explanation, RBT support rating.
- **Well-Being Factors:** Burnout score, work-life balance rating.
- **Turnover Status:** Binary target variable (0 = Stayed, 1 = Left).

### **📈 Exploratory Data Analysis (EDA)**
Key findings from **EDA visualizations**:
- **Higher burnout & lower work-life balance are linked to turnover.**
- **RBTs with more frequent supervision tend to stay longer.**
- **BCBA support & communication ratings impact retention.**

---

## **🤖 Machine Learning Approach**
We experimented with different models to predict turnover risk:

| Model | Accuracy | Recall for Turnover (1) | Precision for Turnover (1) |
|--------|---------|-----------------|-----------------|
| Logistic Regression | 50% | 46% | 27% |
| Random Forest | 63% | 23% | 33% |
| XGBoost (Default) | 59% | 31% | 31% |
| **XGBoost (Threshold 0.4)** ✅ | **57%** | **41%** | **32%** |

### **🚀 Why We Chose XGBoost with Threshold Adjustment**
✅ **Higher recall for turnover cases (`1`)** → 41% (compared to 23% in Random Forest).  
✅ **More balanced predictions** → Detects more RBTs at risk of leaving.  
✅ **Allows early intervention** → Helps clinics take action before turnover happens.  

---

## **📊 Key Visualizations**
The project includes:
- **Feature Correlation Heatmap** → Identifies important turnover-related factors.
- **Feature Importance Plot** → Highlights the most influential variables.
- **Confusion Matrix** → Compares model predictions vs. actual turnover outcomes.

---

## **📂 Repository Structure**
```plaintext
├── README.md               # Project overview & findings
├── data/                   # Dataset files
│   ├── rbt_turnover_data.csv
├── notebooks/              # Jupyter notebooks for analysis
│   ├── eda_rbt_turnover.ipynb    # Data exploration & insights
│   ├── rbt_modeling.ipynb        # Model training & evaluation
├── src/                    # Python scripts for data processing (future)
└── reports/                # Summary reports & presentations
```

## **📍 Next Steps & Future Enhancements** 
🔹 Real-world Data Collection → Integrate actual ABA workforce data.
🔹 Enhanced AI Models → Test deep learning for better turnover predictions.
🔹 Software Integration → Connect predictions with existing ABA management tools.
🔹 User-Friendly Dashboard → Build an interactive tool for BCBA decision-making.

## **📧 Contact**
For questions or collaboration opportunities, feel free to connect with me on LinkedIn or check out my other projects on GitHub.