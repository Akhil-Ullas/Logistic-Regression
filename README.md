# Logistic-Regression


**Logistic regression**
A statistical model used for **binary classification** (e.g., spam/not spam, disease/no disease). It takes numerical inputs, applies a linear combination of features, and pushes the result through a **sigmoid function** to output a probability between 0 and 1. Decision thresholds (commonly 0.5) convert that probability into a class label. It’s simple, interpretable, and works well when classes are linearly separable in feature space.

**Confusion matrix**
A 2×2 table for binary classification showing how predictions match actual labels:

* **TP (True Positive)** – predicted positive, actually positive
* **FP (False Positive)** – predicted positive, actually negative
* **TN (True Negative)** – predicted negative, actually negative
* **FN (False Negative)** – predicted negative, actually positive

It’s the basis for metrics like accuracy, precision, recall, F1-score. If you only use accuracy without checking this matrix, you’re begging to be misled—especially with imbalanced data.

**Why it’s called “regression”**
Because the model **estimates parameters using a regression framework**: it fits a linear function of the inputs. The “regression” part happens before the sigmoid; classification only happens after converting the regression output into a probability. Mathematically, it's a regression on the **log-odds** (logit), not on the class labels themselves.


