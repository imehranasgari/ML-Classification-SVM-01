# SVM Classification on Cell Samples Dataset

## 🎯 Problem Statement and Goal of Project

This project applies a **Support Vector Machine (SVM)** classifier to predict whether a cell sample is **benign** or **malignant**, based on features extracted from cell nucleus characteristics. The primary goal is to explore how SVM handles binary classification problems in medical datasets with potential noise and missing values.

---

## 🛠 Solution Approach

The notebook implements the following workflow:

1. **Data Loading**:

   * Load `cell_samples.csv`, a dataset used for cancer cell classification.
2. **Data Cleaning**:

   * Convert non-numeric column (`BareNuc`) to integers, using `errors='coerce'` to handle invalid entries.
   * Drop rows with missing or non-numeric values.
3. **Visualization**:

   * Plot the relationship between `Clump` and `UnifSize` to visually distinguish between benign and malignant samples.
4. **Feature Selection**:

   * Use 9 nucleus-related attributes as input features (`X`).
   * Define target labels (`Y`) based on class: `2` = benign, `4` = malignant.
5. **Modeling**:

   * Train an **SVM classifier** using `scikit-learn`.
6. **Evaluation**:

   * Evaluate prediction accuracy and visualize decision boundary (optional).

---

## 🧰 Technologies & Libraries

* Python 3
* `pandas`, `numpy` – data handling
* `matplotlib` – basic visualization
* `scikit-learn` – SVM, model evaluation

---

## 📁 Dataset Description

* **File**: `cell_samples.csv`
* **Features**:

  * `Clump`, `UnifSize`, `UnifShape`, `MargAdh`, `SingEpiSize`, `BareNuc`, `BlandChrom`, `NormNucl`, `Mit`
* **Target**:

  * `Class`: 2 (Benign), 4 (Malignant)

This dataset is often used in educational projects for binary classification and SVM model demonstration.

---

## ⚙️ Installation & Execution Guide

1. Make sure the dataset `cell_samples.csv` is placed in the notebook directory.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib scikit-learn
   ```
3. Run the notebook:

   ```bash
   jupyter notebook svm.ipynb
   ```

---

## 📊 Key Results / Performance

* The Support Vector Machine classifier reached an accuracy of 94% on the test set.
* Data cleaning was crucial due to mixed-type columns.
* SVM model successfully learned to distinguish between benign and malignant classes.
* Accuracy scores and visual comparisons (e.g., scatter plots) support the classifier's performance.
* The dataset was successfully cleaned and preprocessed by handling non-numeric entries and removing invalid rows.
* Visual separation between benign and malignant samples was observed in scatter plots.
* The model demonstrates strong performance for binary classification in a medical context.

---

## 📸 Screenshots / Sample Outputs

* ✅ Data cleaning using `pd.to_numeric()` with coercion
* 📈 Scatter plot: `Clump` vs. `UnifSize` by class
* 🧠 Model training using SVM from `scikit-learn`
* 📋 Printed shape of train/test sets

---

## 📚 Additional Learnings / Reflections

* Highlighted importance of data cleaning in medical datasets.
* Demonstrated how **SVM separates non-overlapping classes with a clear margin**.
* This notebook is intended as an educational tool to **illustrate how SVM works**, rather than pushing for highest accuracy or production performance.

---

## 👤 Author

## Mehran Asgari

**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---

