# 🌸 Iris Dataset — KNN Classification

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** on the Iris dataset, identifies and removes less discriminative features, and applies the **K-Nearest Neighbors (KNN)** algorithm to classify iris species for multiple values of *k*.

---

## 🗂 Steps Performed

1. **Load the Dataset**
   - Loaded the built-in Iris dataset from `sklearn.datasets`.
   - Stored features and target in a Pandas DataFrame.

2. **Check for Missing Values**
   - Verified data completeness using `df.isnull().sum()`.
   - **Result:** No missing values were found.

3. **Exploratory Data Analysis (EDA)**
   - **Boxplot:** To detect outliers and compare feature distributions.
   - **Pairplot:** To visualize relationships between features for each class.
   - **Histograms:** To inspect the distribution of each feature.

4. **Feature Selection**
   - Observation: `sepal width` was highly correlated within each class and showed low discriminative power.
   - Action: Removed the `sepal width` column to improve model performance.

5. **Train-Test Split**
   - Split the dataset into **70% training** and **30% testing** using `train_test_split`.

6. **Apply KNN Classifier**
   - Evaluated KNN for different values of *k*: **1, 3, 5, 7, 11**.
   - Recorded accuracy for each *k*.

7. **Plot Results**
   - Plotted model performance (accuracy) against different *k* values for visual comparison.

---

## 📊 Results
- Removing `sepal width` improved class separability.
- Model performance varied with *k*, highlighting the importance of parameter tuning.
- Optimal accuracy was observed at specific *k* values.

---



## 📌 Conclusion
- EDA is essential for understanding feature relevance before modeling.
- Feature removal (`sepal width`) can help improve model discriminative power.
- KNN accuracy depends heavily on the choice of *k*; proper tuning is required for optimal results.
