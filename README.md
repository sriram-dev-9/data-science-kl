# Data Preprocessing & Machine Learning Pipeline

A modular collection of Jupyter Notebooks covering end-to-end data cleaning, feature engineering, and predictive modeling with Python, Pandas, and Scikit-Learn. Built to handle real-world data imperfections systematically before feeding data into a classification pipeline.

---

## Repository Structure

```
.
├── 1 Handling Missing Values.ipynb
├── 2 Deleting Duplicates.ipynb
├── 3 Correcting Inconsistent Formats.ipynb
├── 4 Distance and Similarity.ipynb
└── 5 Week.ipynb
```

Notebooks are sequenced intentionally — work through them in order to go from raw data auditing to a working classifier.

---

## Notebooks

### 1. Handling Missing Values

Strategies for dealing with missing records without introducing statistical skew or losing sample size.

- Detecting null cells (`NaN`)
- Statistical central tendency calculations
- Forward-filling (`ffill`) for sequential/time-series data
- Mean/median imputation (`fillna`) for numeric variables

---

### 2. Deleting Duplicates

Identifies and removes redundant rows that can cause data leakage during training.

- Tracking matching index constraints and primary keys
- Row indexing audits
- Filtering criteria with Pandas DataFrames

---

### 3. Correcting Inconsistent Formats

Standardizes text and date formats across rows into clean, uniform feature schemas.

- Handling datetime parsing variations (e.g., `YYYY-MM-DD` vs `MM/DD/YYYY`)
- Coercing string columns to `datetime64` types

---

### 4. Distance and Similarity Metrics

A mathematical deep-dive into measuring relationships between vectors, text sequences, and spatial data.

- Euclidean, Manhattan, and Minkowski distances
- Hamming distance for categorical/binary data
- Longest Common Subsequence (LCS) for text
- Manual loop implementations vs. SciPy equivalents

---

### 5. Advanced Analysis & Supervised Pipeline

An end-to-end notebook exploring dimensionality reduction and binary classification.

**Dimensionality Reduction**
- PCA (unsupervised) vs. LDA (supervised) — compared side by side

**Statistical Distribution Analysis**
- Skewness and kurtosis inspection on the Iris dataset

**End-to-End Classifier (Titanic dataset)**
- Data collection and feature standardization
- Train/test split and validation
- Logistic Regression classifier
- Evaluation: accuracy, precision, recall, confusion matrix

---

## Setup

**Requirements:** Python 3.12+

```bash
# Clone the repo
git clone https://github.com/sriram-dev-9/data-science-kl.git
cd data-science-kl

# Install dependencies
pip install numpy pandas scipy scikit-learn seaborn matplotlib

# Launch Jupyter
jupyter notebook
```

---

## Suggested Order

| Step | Notebook | Focus |
|------|----------|-------|
| 1 | Handling Missing Values | Data auditing |
| 2 | Deleting Duplicates | Data cleaning |
| 3 | Correcting Inconsistent Formats | Standardization |
| 4 | Distance and Similarity | Metric foundations |
| 5 | Advanced Analysis & Supervised Pipeline | Modeling |

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3.12+-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat&logo=scipy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)
