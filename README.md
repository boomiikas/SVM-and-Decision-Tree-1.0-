# 🌳 SVM and Decision Trees – Experiments

This repository contains experiments with **Support Vector Machines (SVMs)** and **Decision Trees** on synthetic datasets.  
Each question explores classification or regression tasks with different kernels, depths, and evaluation metrics.

---

## 📂 Datasets
- **svm_linear.csv** – 200 rows, 2 features (binary classification, linearly separable).
- **svm_kernel.csv** – 200 rows, 2 features (binary classification, circular pattern).
- **svm_multi.csv** – 300 rows, 2 features, 3 classes (multiclass classification).
- **dt_class.csv** – 200 rows, 2 features + label (classification).
- **dt_depth.csv** – 200 rows, 2 features (classification with varying depth).
- **dt_reg.csv** – 200 rows, 1D regression with noise.

---

## 🔹 Q1) Linear Separability (Binary Classification)
**Dataset:** `svm_linear.csv`

- Train an **SVM with linear kernel** to classify data into 2 classes.  
- Report **accuracy**.  
- Plot **decision boundary** to visualize separation.

---

## 🔹 Q2) Effect of Kernel (Binary Classification)
**Dataset:** `svm_kernel.csv`

- Train **SVM with linear kernel** and **SVM with RBF kernel**.  
- Compare performance on circular pattern data.  
- Report **accuracy difference** and plot decision boundaries.

---

## 🔹 Q3) Multiclass Classification with SVM
**Dataset:** `svm_multi.csv`

- Train **SVM with RBF kernel** for **3-class classification**.  
- Report **accuracy**.  
- Display **confusion matrix** for detailed evaluation.  
- Visualize decision regions.

---

## 🔹 Q4) Simple Classification Tree
**Dataset:** `dt_class.csv`

- Train a **Decision Tree Classifier**.  
- Report **test accuracy**.  
- Visualize the **tree structure**.

---

## 🔹 Q5) Effect of Tree Depth
**Dataset:** `dt_depth.csv`

- Train **Decision Tree Classifier** with depths:
  - `max_depth=2`
  - `max_depth=5`
  - `max_depth=None` (full tree)  
- Compare **train vs test accuracy**.  
- Highlight effect of **overfitting/underfitting**.

---

## 🔹 Q6) Regression Tree
**Dataset:** `dt_reg.csv`

- Train a **DecisionTreeRegressor** to predict target `y` from input `x`.  
- Compare **RMSE** for depths:
  - `max_depth=2`
  - `max_depth=5`
  - `max_depth=None`  
- Visualize regression fit for each depth.

---

## ⚙️ Requirements
- Python 3.x
- NumPy
- Pandas
- Matplotlib / Seaborn
- scikit-learn

---

## 📊 Results & Observations

- **Linear SVM** works well for linearly separable data.  
- **RBF kernel** significantly improves performance on circular data.  
- **Tree depth** strongly affects the bias-variance tradeoff.  
- **Regression trees** with large depth tend to overfit noisy data.  

