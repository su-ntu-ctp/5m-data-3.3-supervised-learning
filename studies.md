# **Self-Study Preparation Guide**

**⏳ Estimated Prep Time:** 45–60 minutes

Welcome to our flipped-classroom session, where you'll review foundational concepts beforehand to maximize our time for hands-on coding and debugging. This pre-study focuses on the critical pillars of the machine learning pipeline: **Preprocessing, Evaluation Metrics, and Model Generalization**.

By familiarizing yourself with these concepts now, we can spend our live session troubleshooting real-world model failures and optimizing pipelines, rather than defining basic terminology. This preparation ensures you are equipped to make high-stakes architectural decisions in your professional data projects.

## ⚡ Your Self-Study Tasks

Please complete the following activities before our session.

### 📝 Task 1: Transforming Raw Data (20 Minutes)

**Activity:** Review the **"Part 1: Preprocessing"** notebook [`part_1_supervised_learning_2_lesson.ipynb`](./notebooks/part_1_supervised_learning_2_lesson.ipynb). Pay close attention to how we handle non-numeric data and why scaling matters for algorithms like SVM and KNN.

**Focus your attention on these key components:**

1. **Categorical Encoding:** The distinction between *Label Encoding* (ordinal) and *One-Hot Encoding* (nominal).
2. **Scaling:** The mathematical difference between *Standardization* (Z-score) and *Normalization*.
3. **Imputation:** Strategies for handling missing values without discarding data.

**Guiding Questions:**

* In a professional setting, if you were processing a column for "Employee Rank" (Junior, Senior, Director), would you use Label Encoding or One-Hot Encoding? Why?
* Why does a model perform poorly if one feature ranges from 0–1 and another ranges from 0–10,000?

### 📝 Task 2: Evaluating Model Performance (20 Minutes)

**Activity:** Read through the **"Classification Metrics"** and **"Regression Metrics"** sections in [`part_2_supervised_learning_2_lesson.ipynb`](./notebooks/part_2_supervised_learning_2_lesson.ipynb). Focus on understanding that "Accuracy" is rarely enough to judge a business-critical model.

**Focus your attention on these key components:**

1. **Confusion Matrix:** The four quadrants (TP, TN, FP, FN).
2. **Precision vs. Recall:** The trade-off between minimizing false positives vs. false negatives.
3. **RMSE vs. MAE:** How different regression metrics penalize large errors.

**Guiding Questions:**

* **Scenario:** You are building a fraud detection system for a bank. Is it more expensive to have a False Positive (flagging a legit transaction) or a False Negative (missing actual fraud)? Which metric optimizes for this?
* How does the ROC Curve help you choose a threshold independent of class distribution?

### 📝 Task 3: The Bias-Variance Tradeoff (20 Minutes)

**Activity:** Skim the **"Part 4: Bias-Variance Tradeoff"** notebook [`part_4_supervised_learning_2_lesson.ipynb`](./notebooks/part_4_supervised_learning_2_lesson.ipynb). Analyze the visual plots showing Underfitting (Degree 1) vs. Overfitting (Degree 15).

**Guiding Questions:**

* If your model performs perfectly on training data but fails miserably on test data, does it suffer from High Bias or High Variance?
* Why might adding *more* features to a model actually hurt its performance in production (overfitting)?

## 🙌🏻 Active Engagement Strategies

To deepen your retention and prepare for our group case study, try one of the following:

* **Scenario Matching:** For Task 2, identify a metric you use (or should use) in your current job/projects. Write down *why* it fits your specific business problem.
* **"Code Commentary":** In the Preprocessing notebook, select the `OneHotEncoder` code block. Write a comment explaining in your own words why `sparse_output=False` might be necessary for visualization but dangerous for memory usage in big data.
* **The "Sweet Spot" Sketch:** Draw a quick graph of the Bias-Variance tradeoff (Total Error vs. Model Complexity) to visualize where the optimal model lies.

## 📖 Additional Reading Material

* [Scikit-Learn: Preprocessing Data](https://scikit-learn.org/stable/modules/preprocessing.html)
* [Scikit-Learn: Precision and Recall Explained](https://scikit-learn.org/stable/auto_examples/model_selection/plot_precision_recall.html)

### 🙋🏻‍♂️ See you in the session!