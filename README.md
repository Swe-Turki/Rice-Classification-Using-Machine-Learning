# Rice Classification Using Machine Learning

This project focuses on classifying rice grains into two distinct varieties — **Gonen** and **Jasmine** — by leveraging machine learning algorithms trained on their morphological and geometric characteristics.

---

## 📁 Project Structure

```
Rice Classification Using Machine Learning/
├── RiceSeed.xlsx                # Excel file containing the dataset
├── dataPrep.py                  # Data cleaning and preprocessing script
├── Py_16.ipynb                  # Jupyter Notebook with model training and evaluation
├── Description of the dataset.pdf  # Dataset and feature description
└── README.md                    # Project documentation
```

---

## 📊 Dataset Overview

The dataset includes **17,490** samples after cleaning (originally 18,185), with the following features describing the rice grains' shape and size.

### Features:

| Feature             | Description |
|---------------------|-------------|
| Area                | Total pixel area of the rice grain |
| Perimeter           | Total boundary length of the grain |
| MajorAxisLength     | Length of the longest axis of the grain |
| MinorAxisLength     | Length of the shortest axis of the grain |
| Eccentricity        | Elongation measure (0 to 1) |
| ConvexArea          | Area of the smallest convex polygon around the grain |
| EquivDiameter       | Diameter of a circle with the same area |
| Extent              | Ratio of Area to bounding box area |
| Solidity            | Ratio of Area to ConvexArea |
| Roundness           | Circularity: 4 * Area / (π * MajorAxisLength²) |
| AspectRatio         | MajorAxisLength / MinorAxisLength |
| Compactness         | Shape uniformity |
| Class               | Target variable: 0 (Gonen), 1 (Jasmine) |

---

## ⚙️ Preprocessing Script

**File:** `dataPrep.py`

Performs the following:

- Missing values are replaced with column means.
- Outliers are removed using the Interquartile Range (IQR) method.
- Duplicates are dropped for data cleanliness.

---

## 📒 Jupyter Notebook

**File:** `Py_16.ipynb`

Includes:

- Data import and exploration
- Preprocessing
- Model training and validation
- Performance metrics visualization (e.g., accuracy, confusion matrix)

---

## 🧰 Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- matplotlib / seaborn
- openpyxl (for reading Excel files)

---

## 🎯 Goal

To classify rice varieties with high accuracy using morphological features, supporting agricultural automation and quality control.

---
