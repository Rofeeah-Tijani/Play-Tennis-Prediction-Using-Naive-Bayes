# Play-Tennis-Prediction-Using-Naive-Bayes

# Project Objective

Predict whether people will play tennis based on weather features using a Naive Bayes classifier.

-----

# Features:

Outlook: Sunny, Overcast, Rain

Temperature: Hot, Mild, Cool

Humidity: High, Normal

Wind: Weak, Strong

Target: PlayTennis (Yes / No) 

------

# Data Encoding Categorical features and the target variable were encoded to numeric values for the model:

| Feature      | Original Values        | Encoded Values |
|-------------|----------------------|----------------|
| Outlook      | Sunny, Overcast, Rain | 2, 0, 1       |
| Temperature  | Hot, Mild, Cool       | 1, 2, 0       |
| Humidity     | High, Normal          | 0, 1          |
| Wind         | Weak, Strong          | 0, 1          |
| PlayTennis   | No, Yes               | 0, 1          |

----

**Model Evaluation**

**Accuracy:** 82.5%

**Confusion Matrix:**

| Actual \ Predicted | No (0) | Yes (1) |
|------------------|--------|---------|
| No (0)           | 11     | 5       |
| Yes (1)          | 2      | 22      |

-----

Model Evaluation

Accuracy: 82.5%

**Classification Metrics**

| Class        | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| No (0)      | 0.85      | 0.69   | 0.76     | 16      |
| Yes (1)     | 0.81      | 0.92   | 0.86     | 24      |
| Accuracy    | —         | —      | 0.825    | 40      |
| Macro Avg   | 0.83      | 0.80   | 0.81     | 40      |
| Weighted Avg| 0.83      | 0.82   | 0.82     | 40      |

-----

## Interpretation:

High recall for Yes (0.92) → model rarely misses playable tennis days.

Precision for Yes = 0.81 → when model predicts Yes, it is correct 81% of the time.

Accuracy = 82.5% → correct predictions for 33 out of 40 test samples.

----

## Key Takeaways

Naive Bayes effectively predicts PlayTennis from categorical weather features.

High recall for Yes → model is strong at detecting playable tennis days.

Encoding categorical variables was necessary for training.

Minor misclassifications (5 false positives, 2 false negatives) are acceptable for this dataset size.

-----







