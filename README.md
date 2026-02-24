# Diabetes-Risk-Classification
 

# Project Overview

This project focuses on predicting whether a patient is **diabetic ,pre-diabetic or non-diabetic** using clinical and demographic features. The goal was to build an interpretable machine learning model that can support data-driven healthcare decision-making.

A **Decision Tree Classifier** was selected due to its transparency and ability to capture non-linear relationships while remaining easy to interpret.

# Objective

* Build a classification model for diabetes prediction
* Control model complexity to prevent overfitting
* Evaluate performance using appropriate classification metrics
* Interpret model decisions to understand key risk factors

# Dataset

The dataset contains clinical diagnostic measurements including:

* Pregnancies
* Glucose
* Blood Pressure
* Skin Thickness
* Insulin
* BMI
* Diabetes Pedigree Function
* Age

Target variable:

* `0` - Non-diabetic
* `1` - pre-diabetic
* `2` - Diabetic

# Methodology

#  Data Preparation

* Separated features and target variable
* Split data into training and testing sets (80/20 split)
* No scaling applied (Decision Trees do not require feature normalization)

# Model Selection

A **Decision Tree Classifier** was chosen because:* It is interpretable,* Handles non-linear relationships,* Requires minimal preprocessing

# Overfitting Control

To improve generalization:

* Limited `max_depth`
* Set `min_samples_split`
* Set `min_samples_leaf`

This helped manage the bias–variance tradeoff.

# Model Evaluation

Performance was evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* Confusion Matrix


# Results

The model achieved solid classification performance and demonstrated strong predictive power for identifying diabetes risk.

Key findings:

* Glucose levels and BMI were strong predictors.
* Controlling tree depth significantly reduced overfitting.
* The model performed well in identifying non-diabetic cases, with some false negatives observed.

The confusion matrix provided insight into prediction errors, which is especially important in healthcare contexts where false negatives carry higher risk.

# Key Learnings

* Decision Trees are highly interpretable but prone to overfitting.
* Hyperparameter tuning is critical for generalization.
* Model evaluation must go beyond accuracy in medical datasets.
* Feature importance analysis provides actionable insights.


# Technologies Used:Python,NumPy,Matplotlib,scikit-learn

# Conclusion

This project demonstrates the practical application of supervised machine learning in healthcare. By carefully controlling model complexity and focusing on interpretability, the Decision Tree model provided meaningful insights into diabetes risk factors while maintaining strong predictive performance.


