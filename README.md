# Comparative Study: Decision Trees vs. Linear Models

This repository explores the performance trade-offs between Tree-based models and Linear models across two distinct domains: Healthcare (Classification) and Automotive Engineering (Regression).

##  Comparison Summary

| Task | Dataset | Model A (Linear) | Model B (Tree) |
| :--- | :--- | :--- | :--- |
| **Classification** | Wisconsin Breast Cancer | Logistic Regression | Decision Tree Classifier |
| **Regression** | Auto-MPG | Linear Regression | Regression Tree |

---

##  Project 1: Breast Cancer Diagnostic (Classification)
**Goal:** Classify tumors as Benign (0) or Malignant (1).
- **Core Strategy:** Comparing the linear decision boundary of Logistic Regression against the non-linear "splitting" logic of a Decision Tree.
- **Result:** Even using only 2 features (`radius_mean` and `concave points_mean`), the Decision Tree identifies complex patterns that a straight line might miss.

##  Project 2: Auto-MPG Efficiency (Regression)
**Goal:** Predict a vehicle's miles-per-gallon (MPG) consumption.
- **Core Strategy:** Testing if automotive performance follows a linear trend or a hierarchical structure.
- **Key Discovery:** Using 6 technical features, the Regression Tree captures non-linear interactions (e.g., how horsepower and weight combined affect fuel) more flexibly than standard Linear Regression.

---

##  Environment Setup (Conda)

### 1. Create the Environment
```bash
git clone https://github.com/Joe-Naz01/ml_tree.git
cd ml_tree

conda create -n ml_tree
conda activate ml_tree

pip install requirements.txt
