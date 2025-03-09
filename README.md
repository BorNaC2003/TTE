# **Enhancing Target Trial Emulation with Clustering**  

## **Project Contributors**  
**Nathaniel Castro Borces**  
**Anthony Cid Mendoza**  

## **Objective**  
This project explores how clustering techniques can be integrated into **Target Trial Emulation (TTE)** to improve causal inference in observational studies. By applying methods like **K-Means** and **DBSCAN**, we aim to reduce biases and enhance treatment effect estimation.  

Key steps include:  
1. **Converting R-based TTE code to Python** while ensuring accurate replication.  
2. **Incorporating clustering algorithms** to refine model accuracy.  
3. **Analyzing clustering’s impact** on performance metrics and survival predictions.  

## **Project Workflow**  

### **1. Data Collection & Preparation**  
- Download the dataset from **[this source](https://rpubs.com/alanyang0924/TTE)**.  
- Extract the data and save it as **`data_censored.csv`**.  

### **2. Code Translation & Validation**  
- Convert the existing **R implementation** to **Python** using **Jupyter Notebook**.  
- Ensure the results remain consistent with the original framework.  

### **3. Integrating Clustering Techniques**  
- Create a new version of the Python implementation (**TTE-v2.ipynb**).  
- Identify key points in the **TTE process** where clustering can be applied.  
- Implement **K-Means clustering** and examine its impact on bias reduction.  
- Explore alternative clustering methods such as **DBSCAN, Gaussian Mixture Models (GMM), or Hierarchical Clustering**.  

### **4. Refining Weight Adjustments**  
- Use **cluster labels** to improve **treatment switching** and **censoring weight models**.  
- Compute **Inverse Probability Weights (IPWs)** with clustering considerations.  

### **5. Modeling Outcomes & Predicting Survival**  
- Develop a **logistic regression model** to predict treatment outcomes.  
- Measure model effectiveness using **McFadden’s Pseudo \(R^2\)**.  
- Utilize a **Marginal Structural Model (MSM)** for survival analysis.  

### **6. Evaluating Model Performance**  
- Compare different approaches using:  
  - **Akaike Information Criterion (AIC) & Bayesian Information Criterion (BIC)**.  
  - **ROC-AUC scores** for model classification performance.  
  - **Cross-validation** to assess robustness.  
- Visualize the impact of clustering on survival predictions.  
