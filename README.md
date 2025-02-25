![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

# Applied AI Group Project 1

### **Project Overview**
This repository hosts a collaborative project for the Applied Artificial Intelligence course (AAI-500-03), focusing on probability and statistical analysis in AI. Our current project aims to predict obesity levels using data from the UCI Machine Learning Repository.

### **About the Obesity Dataset**
The dataset contains demographic, anthropometric, dietary, and behavioral attributes to explore the relationship between obesity and various genetic, lifestyle, and dietary factors.
1. Our analysis includes:
2. Generating Hypotheses
3. Data Cleaning & Preparation
4. Exploratory Data Analysis (EDA)
5. Descriptive Analytics
6. Predictive Analytics, featuring:
   - Model Selection
   - Model Analysis
   - Conclusion & Recommendations

### **Branches in the Repository**
- **main**: Contains the final files, folder structure, and environment configurations.
- **stagebranch**: Used for most of the commits, experimental implementations, and updates.

---

### **Getting Started**
**1. Clone the Repository**
```
git clone <https://github.com/clappy203/Applied-AI-Group-Projects/tree/stagebranch>
```

**2. Install Dependencies through Vs.code Terminal (if applicable)**
   ```
  pip install requirements.txt
  ```

**3. Ensure Jupyter Notebook is Installed**
      If Jupyter is not installed

**7. Run Jupyter Notebook in vscode**
      Navigate to the data_analysis_new.ipynb file to begin exploring the dataset.
---

### Data Exploration and Prediction

**1. Hypothesis Generation**
We formulate hypotheses to analyze the relationship between obesity and factors such as genetic predisposition, smoking, alcohol consumption, and physical activity.

**2. Data Cleaning & Preparation**
- Convert categorical variables
- Normalize/standardize data

**3. Exploratory Data Analysis (EDA)**
- Visualize obesity distribution across age, gender, and lifestyle factors
- Correlation analysis to ensure independent contributions

**4. Descriptive Analytics**
- Summary statistics to understand data distribution
- Multivariate Analysis
- Principal Component Analysis (PCA) to identify feature importance and linear relationship

**5. Predictive Analytics**
- Train various machine learning models:
  - One-vs-One Logistic Regression (baseline model)
  - Decision Trees
  - Random Forest
  - Support Vector Machines (SVM)
  - XGBoost (best performing model, 94.80% accuracy)
- Model evaluation using accuracy, log-loss, and feature importance

**6. Model Analysis & Insights**
- **Key Findings:**
- Genetic predisposition and unhealthy lifestyle contribute significantly to obesity.
- PCA reveals distinct yet overlapping obesity clusters.
- XGBoost outperforms other models due to its boosting mechanism and ability to capture complex relationships.

**7. Conclusion & Recommendations**
- Data-driven interventions are crucial to mitigating obesity risk.
- Future research should incorporate longitudinal data for causal inference.
---------

### **Project Management**
Kanban Board: https://github.com/users/clappy203/projects/1/views/1

