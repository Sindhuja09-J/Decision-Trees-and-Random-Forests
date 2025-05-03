# 🌳 Decision Tree and Random Forest Classification on Heart Disease Dataset

This project demonstrates how to apply **Decision Tree** and **Random Forest** classifiers on a medical dataset to predict heart disease. It includes training, visualization, feature analysis, and evaluation using cross-validation. Additionally, it investigates model overfitting by varying tree depth.

---

## 📂 Project Structure

- ✅ Train and visualize a **Decision Tree**
- 🔁 Analyze model performance at different tree depths (overfitting vs. generalization)
- 🌲 Train and evaluate a **Random Forest**
- 📊 Plot and interpret **feature importances**
- 📈 Evaluate both models using **cross-validation**
- 🧾 Generate a classification report

---

## 🧰 Libraries Used

- `pandas` – Data manipulation
- `numpy` – Numerical operations
- `matplotlib`, `seaborn` – Visualization
- `sklearn` – Models and metrics:
  - `DecisionTreeClassifier`
  - `RandomForestClassifier`
  - `train_test_split`, `cross_val_score`
  - `classification_report`
  - `plot_tree`

---

## 📊 Dataset

The dataset used is a heart disease dataset in CSV format named `heart.csv`, containing various medical features and a target column indicating disease presence (`target`).

---

## ⚙️ How It Works

1. **Load and Prepare Data**
   - Read CSV into a DataFrame
   - Split into features (`X`) and label (`y`)
   - Train-test split (80-20)

2. **Train a Decision Tree**
   - Fit on training data
   - Predict on test data
   - Print accuracy

3. **Visualize the Tree**
   - Use `plot_tree()` from `sklearn.tree` to display the structure

4. **Analyze Overfitting**
   - Loop through tree depths (1–14)
   - Record training and test accuracy
   - Plot the results to visualize underfitting vs. overfitting

5. **Train a Random Forest**
   - Use 100 trees with a fixed random state
   - Compare accuracy with Decision Tree

6. **Feature Importance**
   - Extract and plot top features influencing the prediction

7. **Cross-Validation**
   - Use 5-fold cross-validation for both models
   - Compare mean accuracy scores

8. **Classification Report**
   - Precision, recall, and F1-score for the Random Forest model

---

## 📈 Output Visuals

- Decision Tree Plot (simple, interpretable splits)
- Overfitting Analysis Graph (accuracy vs. depth)
- Bar Plot of Feature Importances
