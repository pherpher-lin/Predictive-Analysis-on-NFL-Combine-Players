# NFL Combine Analysis — Running Back Performance Study

## Overview
This project analyzes NFL Combine performance metrics for running backs to determine whether physical testing results can reliably predict NFL success. The analysis used combine measures such as 40-yard dash time, bench press reps, vertical jump height, and player weight, and compared them against rushing yard performance and classification into “Elite” vs. “Non-Elite” players. Data was sourced from NFL Combine historical datasets.

## Tools & Techniques Used
- **Python (Pandas, NumPy)** for cleaning and filtering player data  
- **Scikit-Learn** for building linear models, classification models, and clustering  
- **Matplotlib / Seaborn** for visualizations  
- **Machine Learning Models**:
  - Linear Regression  
  - Logistic Regression  
  - K-Means Clustering  

All dataset preparation, model training, and result evaluation were performed through Python-based workflows.  
*(Source: Project Report)*

## Key Results

### Linear Regression
**Goal:** Predict rushing yards from combine metrics  
- Multivariate Model R² ≈ **-0.87**  
- Single-metric Model R² ≈ **-0.38**

**Interpretation:**  
Combine performance does not meaningfully predict rushing yard totals. The negative R² values indicate worse-than-baseline performance.

---

### Logistic Regression
**Goal:** Classify players as Elite or Non-Elite  
- Model Accuracy: **95%**  
- Recall for Elite players: **Very low**

**Interpretation:**  
The model accurately labeled non-elite players but failed to detect elite players. The confusion matrix showed **zero correct predictions** for elite classification.

---

### K-Means Clustering
**Goal:** Group players based on performance features  
- Accuracy: **34%**  
- Recall: **34%**

**Interpretation:**  
Players do not naturally separate into clear performance tiers using combine metrics alone.

---

## Key Takeaways
- Combine performance shows weak predictive value for NFL success.
- Classification models leaned toward predicting average-tier players.
- Clustering confirms that combine metrics alone are poor differentiators.
- Combine drills do not reliably highlight elite running back performance.
