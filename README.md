# 🧠 Employee Attrition Prediction (IBM HR Analytics)

This project predicts **employee attrition** (whether an employee will leave or stay) using the IBM HR Analytics dataset.
It uses basic data cleaning, one‑hot encoding, and a **Logistic Regression** baseline trained/tested on an 80/20 split.

> This README is a starter template. Update the **Results** section with your exact metrics after you run the notebook.

---

## 📁 Project Contents
- `employee_attrition_model.ipynb` — Jupyter notebook with the full analysis and model
- `requirements.txt` — minimal Python dependencies
- `.gitignore` — ignores large/temporary files on GitHub

---

## ⚙️ How to Run
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
2. Open the notebook:
   ```bash
   jupyter notebook employee_attrition_model.ipynb
   ```
3. (Optional) Place the dataset CSV as `WA_Fn-UseC_-HR-Employee-Attrition.csv` in the **same folder** or adjust the path in the notebook accordingly.

---

## 📊 Results (update these with your actual numbers)
- Accuracy: `0.xx`
- Precision: `0.xx`
- Recall: `0.xx`
- F1‑score: `0.xx`

**Notes:** I used `class_weight="balanced"` to improve recall on the minority class (attrition = 1).

---

## 🔍 Key Insights (example; edit after you run)
- Overtime and lower job satisfaction are associated with higher attrition risk.
- Balanced logistic regression improved recall compared to the default model.

---

## 🧰 Tech Stack
Python · Pandas · scikit‑learn · Matplotlib · Jupyter

---

© 2025 Stephanie A. Danquah
