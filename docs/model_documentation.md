
## 📋 Model Summary & Evaluation

- **Model**: RandomForestClassifier
- **Dataset**: Iris (3-class classification)
- **Accuracy**: [Can add from model.score() if desired]

## 🔍 SHAP Findings

- Top Features Globally:
  - Petal width (cm)
  - Petal length (cm)
- SHAP waterfall shows how each feature pushes prediction up or down.

## 🧠 LIME Insights

- LIME explained individual prediction by highlighting:
  - Conditions like `petal width > x` or `sepal length < y`
  - Impact values (positive/negative contributions)
