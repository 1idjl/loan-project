# Loan Prediction Machine Learning Project

This project predicts loan approval using various machine learning models. It includes data preprocessing, feature engineering, model training, evaluation, and comparison.

## 📁 Project Structure

```
loan-project/
├── data/
│   ├── loan.csv
│   ├── processed/
│   └── raw/
├── notebooks/
│   ├── data2.ipynb
│   ├── best_ANN (MLP)_model.pkl
│   ├── best_CatBoost_model.pkl
│   ├── best_KNN_model.pkl
│   ├── best_LightGBM_model.pkl
│   ├── best_loan_prediction_model.pkl
│   ├── best_LogisticRegression_model.pkl
│   ├── best_RandomForest_model.pkl
│   ├── best_SVM_model.pkl
│   ├── best_voting_classifier.pkl
│   ├── best_XGBoost_model.pkl
│   ├── comparison_accuracy.html
│   ├── comparison_f1-score.html
│   ├── comparison_precision.html
│   ├── comparison_recall.html
│   └── ...
├── src/
│   └── ...
├── tests/
│   └── ...
├── requirements.txt
├── README.md
```

## 🚀 How to Run

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/loan-project.git
   cd loan-project
   ```

2. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

3. **Run Jupyter Notebook for analysis and modeling:**
   ```sh
   jupyter notebook notebooks/data2.ipynb
   ```

## 🧹 Data Preprocessing

- Missing values handled using KNNImputer.
- Features encoded and scaled.
- Outliers removed using IQR method.
- Feature engineering: `TotalIncome`, `LTI`, `DTI`.

## 🏦 Modeling

- Models trained: Logistic Regression, KNN, ANN (MLP), Random Forest, XGBoost, LightGBM, CatBoost, SVM.
- Hyperparameter tuning with GridSearchCV/RandomizedSearchCV.
- SMOTE used for class balancing.
- VotingClassifier combines top models.

## 📊 Evaluation & Visualization

- Metrics: Accuracy, Precision, Recall, F1-Score, ROC AUC.
- Comparison charts saved as HTML: accuracy, precision, recall, f1-score.
- Feature importance visualized.
- ROC curves for all models.

## 📦 Outputs

- Best models saved as `.pkl` files in `notebooks/`.
- Evaluation results saved as CSV and HTML.

## 📝 License

MIT License.

---

**For more details, see the notebook:** [notebooks/data2.ipynb](notebooks/data2.ipynb)