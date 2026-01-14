# One-Hot-Encodding

# One-Hot Encoding in Machine Learning (Scikit-Learn)

## 📌 Topic: One-Hot Encoding

One-Hot Encoding is a **data preprocessing technique** used to convert **categorical variables** into a numerical format so that machine learning algorithms can process them effectively.

---

## 📖 What is One-Hot Encoding?

One-Hot Encoding creates **binary columns** for each category in a categorical feature.

### Example:

| Color | Red | Blue | Green |
|------|-----|------|-------|
| Red  | 1   | 0    | 0     |
| Blue | 0   | 1    | 0     |
| Green| 0   | 0    | 1     |

Each category becomes a separate column with values `0` or `1`.

---

## 🎯 Why Use One-Hot Encoding?

- Machine learning models require **numerical input**
- Prevents **false ordinal relationships**
- Works well with:
  - Linear Regression
  - Logistic Regression
  - Decision Trees
  - Random Forest
  - Gradient Boosting

---

## ⚠️ When NOT to Use One-Hot Encoding?

- When the feature has **many unique categories** (high cardinality)
- When categories have a **natural order** (use Ordinal Encoding instead)

---

## 🧠 One-Hot Encoding vs Ordinal Encoding

| Feature | One-Hot Encoding | Ordinal Encoding |
|-------|------------------|------------------|
| Order matters | ❌ No | ✅ Yes |
| Output | Multiple columns | Single column |
| Use case | Nominal data | Ordered categories |

---

## 📦 Required Libraries

```python
import numpy as np
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import OneHotEncoder
