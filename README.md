# Predicting Credit Card Customer Attrition and Clustering Similar Customers  

This project analyzes a dataset of 10,000 credit card customers to predict customer attrition and group similar customers using clustering techniques. The dataset includes features such as age, salary, and card category.  

## Dataset  
- **Source**: [Kaggle - Credit Card Customers](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers?select=BankChurners.csv)  
- Contains 22 features related to customer demographics, behavior, and account details.  

## Project Workflow  

### Data Preprocessing  
1. Removed unknown values and encoded categorical variables.  
2. Scaled features using StandardScaler (except for Random Forest).  
3. Applied stratified sampling for training/testing split due to class imbalance.  

### Supervised Learning  
- **Objective**: Predict customer attrition using the `Attrition_Flag` column.  
- Models Used:  
  - Logistic Regression  
  - Random Forest  
  - Support Vector Machine (SVM)  
- **Best Model**: Random Forest with an F1 score of 0.875, outperforming others in precision and recall.  

### Unsupervised Learning  
- **Objective**: Cluster similar customers using K-means clustering.  
- **Dimensionality Reduction**: Principal Component Analysis (PCA) to reduce noise and irrelevant features.  
- **Evaluation Metrics**:  
  - Silhouette Score  
  - Davies-Bouldin Score  

## Key Findings  
1. **Supervised Models**: Random Forest captured non-linear relationships and provided the most balanced performance.  
2. **Clustering**: PCA improved clustering scores but revealed challenges in achieving distinct cluster separations due to dataset characteristics.  

## Future Work  
1. Explore alternative clustering algorithms (e.g., DBSCAN) for non-spherical clusters.  
2. Investigate additional dimensionality reduction techniques. 
