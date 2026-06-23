# Univariate and Multivariate Analysis — Seaborn Diamonds Dataset

## Overview
This Jupyter Notebook performs exploratory statistical analysis on the **seaborn `diamonds` dataset** (53,940 diamonds with 10 features).

## Variables Analyzed
| Analysis Type | Variable(s) |
|---|---|
| **Univariate** | `price` (USD) |
| **Multivariate** | `carat` × `price`, grouped by `cut` |

## What's Inside
### Univariate Analysis (`price`)
- Descriptive statistics (mean, median, std, skewness, kurtosis)
- D'Agostino-Pearson normality test
- 4-panel visual dashboard: Histogram + KDE, Box Plot, Violin Plot, Q-Q Plot

### Multivariate Analysis (`carat` × `price` × `cut`)
- Pearson correlation coefficient
- Full numeric correlation matrix
- 4-panel visual dashboard: Scatter plot, Regression lines by cut, Box plots by cut, Correlation heatmap

## Requirements
```bash
pip install numpy pandas seaborn matplotlib scipy notebook
```

## Usage
```bash
jupyter notebook "Univariate_and_Multivariate_Analysis.ipynb"
```

## Key Findings
- **Price** is strongly right-skewed (median $2,401 vs mean $3,933) and non-normal
- **Carat vs Price** has a strong positive correlation (r ≈ 0.92) — carat weight is the dominant price driver
- **Cut quality** has a secondary and sometimes paradoxical effect on price due to confounding with carat weight
