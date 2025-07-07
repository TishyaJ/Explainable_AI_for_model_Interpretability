# 🔍 Explainable AI for Model Interpretability

This project demonstrates an **Explainable AI (XAI) framework** that helps interpret the decisions made by a machine learning model. The framework provides visual and textual insights into how the model arrives at its predictions — making it more transparent and trustworthy.

---

## 💡 Objective

> Develop an explainable AI system to interpret predictions made by a classifier trained on the Iris dataset using **SHAP** and **LIME**.

---

## 🧠 Model Summary

- **Model Used**: `RandomForestClassifier`
- **Dataset**: Iris (3-class classification)
- **Accuracy**: `100%` on test set
- **Saved Model**: [`model/random_forest_model.joblib`](model/random_forest_model.joblib)

---

## 🔎 Interpretability Tools

### ✅ SHAP (SHapley Additive exPlanations)
- Visualizes **global** feature importance and individual prediction breakdowns.
- Output:
  - ![SHAP Beeswarm](model/shap_beeswarm_class0.png)

### ✅ LIME (Local Interpretable Model-Agnostic Explanations)
- Provides **local** explanations for a single prediction.
- Output:
  - Interactive HTML file (`lime_explanation.html`) — **not uploaded to GitHub**, but available locally.

---
## 🚀 How to Use

1. Clone the repo and open the notebook.
2. Train the model or load the saved one.
3. Generate SHAP and LIME explanations.
4. Explore:
   - `docs/model_documentation.md` for summary.
   - `model/shap_beeswarm_class0.png` for SHAP visuals.
   - `lime_explanation.html` for LIME results (open in browser).

---

## ✍️ Author

**Tishya Jha**  
B.Tech. CSE (Design) @ RGIPT  
🔗 [GitHub](https://github.com/TishyaJ)

---

## 📜 License

This project is licensed under the MIT License.
