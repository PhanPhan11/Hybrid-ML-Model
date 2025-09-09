# Hybrid-ML-Model
# Hybrid Machine Learning Model for Financial Health Classification  

Final Project – University of Economics and Law (UEL), Vietnam National University HCMC  
Subject: Machine Learning and Artificial Intelligence in Finance  
Author: Phan Thị Thu Huyền  

---

## Project Overview  
Financial distress and corporate failure can result in significant social and economic costs. This project develops a hybrid machine learning framework to classify and predict the financial health of companies based on financial ratios.  

Traditional statistical models such as logistic regression have limitations in predictive power. By integrating clustering (unsupervised learning) with classification (supervised learning), this study aims to enhance both prediction accuracy and interpretability.  

---

## Key Features  
- **Dataset:** Financial statements (2021–2024) of 1,547 Vietnamese companies.  
- **Preprocessing:** Data cleaning, handling missing values, standardization, and financial ratio calculations.  
- **Dimensionality Reduction:** Applied PCA to reduce from 11 ratios to 2 principal components for visualization and to address multicollinearity.  
- **Clustering Algorithms Evaluated:**  
  - DBSCAN (low cluster separation)  
  - DBSCAN + KMeans (moderate improvement)  
  - Gaussian Mixture Model (weak separation)  
  - HDBSCAN (best performance, Silhouette Score = 0.6431)  
- **Classification Algorithms:**  
  - Random Forest – Accuracy: 91.8% (biased toward majority class)  
  - XGBoost – Accuracy: 94.3%, strong performance across all classes  

---

## Results and Insights  
- **Cluster Profiles:**  
  - Healthy firms: strong ROA, ROE, liquidity, and low leverage  
  - Moderate firms: average ratios with higher reliance on debt  
  - Weak firms: low liquidity, weak profitability, financial stress  
- **Historical Application (2021–2023):**  
  - Approximately 68% of firms classified as Healthy  
  - Higher financial risk identified in Travel & Leisure and Industrial Services  
  - Defensive sectors such as Healthcare and Chemicals showed resilience  

---

## Methodology and Tools  
- **Programming Language:** Python  
- **Libraries:** Pandas, Scikit-learn, XGBoost, Matplotlib, Seaborn  
- **Algorithms:** HDBSCAN, PCA, Random Forest, XGBoost  
- **Evaluation Metrics:** Silhouette Score, Calinski-Harabasz Index, classification report  

---

## Practical Implications  
- Supports investors in credit risk assessment and portfolio management  
- Provides policy makers with tools for monitoring financial stability  
- Offers early warning indicators for potential corporate distress  

---

## How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/financial-health-ml.git
   cd financial-health-ml
