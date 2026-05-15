# DSV - Lab7

*Introduction to Data Science and Visualization*

You can find two cheat sheet in this repo:
- model_selection_cheatsheet.md contains the available models and the required preprocessing
- preprocessing_cheatsheet.md helps you choose a preprocessing technique and apply it correctly to the data. 

May 8, 2026

## Learning objectives

By the end of this lab you will be able to:

1. Identify and prevent **data leakage** (target leakage, preprocessing leakage, target encoding leakage).
2. Detect **train/test contamination** caused by duplicates or by ignoring time.
3. Choose **appropriate metrics** for imbalanced classification.
4. Pick a **cross-validation scheme** that matches the data structure.
5. Avoid **selection bias** when tuning hyperparameters.
6. Understand the difference between **probabilities and class predictions**, and tune the decision threshold.

> *In machine learning, getting a high test score is easy — the hard part is getting a high score for the right reason.*


## Dataset Schema

| Column | Type | Description |
|---|---|---|
| `transaction_id` | int | Unique transaction identifier *(mostly)* |
| `timestamp` | datetime | When the transaction happened |
| `customer_id` | int | Who made the transaction |
| `amount` | float | Transaction amount in EUR |
| `category` | str | Merchant category (`grocery`, `gas`, `online`, …) |
| `hour` | int | Hour of day (0–23) |
| `distance_from_home` | float | Distance between merchant and cardholder home (km) |
| `days_since_last` | float | Days since the customer's previous transaction |
| `fraud_review_status` | str | Status from the bank's review system |
| `is_fraud` | int | **Target.** 1 = confirmed fraud, 0 = legitimate |





