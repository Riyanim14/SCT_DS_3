# 🏦 Bank Term Deposit Prediction using Decision Tree Classifier

This project uses a **Decision Tree Classifier** to predict whether a client will subscribe to a term deposit based on various client and campaign-related features. The dataset is based on direct marketing campaigns (phone calls) of a Portuguese banking institution.

---

## 📂 Dataset

- **Source:** [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/Bank+Marketing)
- **File:** `bank.csv`
- **Separator:** `;`
- **Target Column:** `deposit` (`yes` or `no`)

---

## 🔧 Features Used

Includes both numeric and categorical features such as:
- Age, Job, Marital status, Education
- Default, Housing, Loan
- Contact type, Month, Duration, Campaign performance
- Previous outcomes, Balance, etc.

---

## 🧠 ML Model

- **Model:** `DecisionTreeClassifier` from `scikit-learn`
- **Max Depth:** 5
- **Train/Test Split:** 70/30 (Stratified)

---

## ✅ Pipeline Steps

1. Load dataset with correct separator.
2. Strip whitespace from column names.
3. Encode categorical variables using `LabelEncoder`.
4. Split the dataset with `train_test_split` (stratified).
5. Train a Decision Tree Classifier.
6. Evaluate model using:
   - Accuracy
   - Classification report
   - Confusion matrix
7. Visualize:
   - Confusion matrix heatmap
   - Feature importance bar chart
   - Enhanced decision tree plot

---

## 📈 Results

- **Accuracy:** ~80%
- **Balanced Precision/Recall:** for both `yes` and `no` classes
- **Visualization:** Colorful and intuitive decision tree with rounded boxes, proportions, and impurity shown.

---

## 📊 Visualizations

- Confusion Matrix (Seaborn heatmap)
- Feature Importance Plot
- Enhanced Decision Tree using `plot_tree` with:
  - Proportions
  - Rounded Nodes
  - Color gradients based on class purity

---

## 📎 Requirements

```bash
pip install pandas scikit-learn matplotlib seaborn graphviz
