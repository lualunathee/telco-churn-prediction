# Customer Churn Prediction & Retention Strategy

Predicting which telecom customers are likely to leave, and turning those predictions into retention decisions.

**Dataset:** [Telco Customer Churn (Kaggle)](https://www.kaggle.com/blastchar/telco-customer-churn): 7,043 customers, 21 features
**Tools:** Python, pandas, NumPy, scikit-learn, matplotlib

## What's inside

| Part | What was done |
|---|---|
| Probability analysis | Overall, conditional and joint churn probabilities, lift, top predictive features |
| Model | Gaussian Naive Bayes **implemented from scratch** in NumPy, evaluated with accuracy, precision, recall, F1, ROC/AUC and calibration, compared with scikit-learn |
| Business decisions | Expected value of retention, risk/value segmentation, budget optimization, sensitivity analysis |

## Key results

- Overall churn rate: **26.5%**
- Highest-risk segment, Month-to-month contract + Fiber optic: **54.6% churn (lift 2.06)**
- From-scratch Naive Bayes: **AUC 0.807**, **recall 0.84**, accuracy 0.69 (same as scikit-learn GaussianNB)
- **High Value / High Risk** customers give the best return on retention spend
- With a 50,000 budget: target **166 customers** for about **83,000 expected profit**
- Profit is most sensitive to the retention offer's success rate

## How to run

```bash
pip install -r requirements.txt
jupyter notebook churn_prediction.ipynb
```

Put `WA_Fn-UseC_-Telco-Customer-Churn.csv` (from the Kaggle link above) in the same folder as the notebook.

---
*Completed as Lab 4 of the Data Storage and Analysis course, KBTU, Spring 2026.*
