![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=GitHub&logoColor=white) ![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

# Applied AI Group Project 1

### **Project Overview**
This repository hosts a collaborative project for the Applied Artificial Intelligence course (AAI-500-03), focusing on probability and statistical analysis in AI. Our current project aims to predict obesity levels using data from the UCI Machine Learning Repository.

### **About the Obesity Dataset**
The dataset contains demographic, anthropometric, dietary, and behavioral attributes to explore the relationship between obesity and various genetic, lifestyle, and dietary factors.Our analysis includes:
1. Generating Hypotheses
2. Data Cleaning & Preparation
3. Exploratory Data Analysis (EDA)
4. Descriptive Analytics
5. Predictive Analytics, featuring:
   - Model Selection
   - Model Analysis
   - Conclusion & Recommendations

### **Repository Structure**
```plaintext
Applied-AI-Projects/
│-- README.md
│-- LICENSE
│-- .gitignore
│-- poetry.lock
│-- poetry.toml
│-- aai_project/
│   ├── .virtual_documents/
│   ├── aai_project/
│   ├── data/ (Holds the obesity dataset)
│   ├── notebooks/ (Jupyter notebooks for analysis)
│   │   ├── data_analysis.ipynb
```

### **Branches in the Repository**
- **main**: Contains the final files, folder structure, and environment configurations.
- **stagebranch**: Used for most of the commits, experimental implementations, and updates.

---

### **Getting Started**
**1. Clone the Repository**
```
git clone <https://github.com/clappy203/Applied-AI-Group-Projects/tree/main>

cd aai_propject
```

**2. Install Poetry (If Not Installed)**
    Poetry is used to manage dependencies and the virtual environment.
```
curl -sSL https://install.python-poetry.org | python3 -
export PATH="$HOME/.local/bin:$PATH"

poetry --version
```

**3. Install Dependencies**
Run the following command inside the project directory:
```
poetry install
```
This will install all required libraries from pyproject.toml.

**4. Activate the Poetry Environment**
```
poetry shell
```

**5. Ensure Jupyter Notebook is Installed**
If Jupyter is not installed, run:
```
poetry run pip install notebook
```

**6. Add Poetry Environment to Jupyter Kernel**
```
poetry run python -m ipykernel install --user --name=poetry-env --display-name "Python (Poetry)"
```
verify with:
```
jupyter kernelspec list
```

**7. Run Jupyter Notebook**
```
poetry run jupyter notebook
```
Navigate to the notebooks folder and open data_analysis.ipynb to begin exploring the dataset.

---

### Data Exploration and Prediction

**1. Hypothesis Generation**
We formulate hypotheses to analyze the relationship between obesity and factors such as genetic predisposition, smoking, alcohol consumption, and physical activity.

**2. Data Cleaning & Preparation**
- Handle missing values
- Convert categorical variables
- Normalize/standardize data if necessary

**3. Exploratory Data Analysis (EDA)**
- Visualize obesity distribution across age, gender, and lifestyle factors
- Correlation analysis to ensure independent contributions

**4. Descriptive Analytics**
- Summary statistics to understand data distribution
- Principal Component Analysis (PCA) to identify feature importance

**5. Predictive Analytics**
- Train various machine learning models:
  - One-vs-One Logistic Regression (baseline model)
  - Decision Trees
  - Random Forest
  - Support Vector Machines (SVM)
  - XGBoost (best performing model, 94.80% accuracy)
- Model evaluation using cross-validation (CV) score, accuracy, log-loss, and feature importance

**6. Model Analysis & Insights**
- **Key Findings:**
- Genetic predisposition and unhealthy lifestyle contribute significantly to obesity.
- PCA reveals distinct yet overlapping obesity clusters.
- XGBoost outperforms other models due to its boosting mechanism and ability to capture complex relationships.

**7. Conclusion & Recommendations**
- Data-driven interventions are crucial to mitigating obesity risk.
- Future research should incorporate longitudinal data for causal inference.

---

### Summary of Commands
```
# Clone the repository
git clone <repository-url>
cd Applied-AI-Projects

# Install Poetry (if not already installed)
curl -sSL https://install.python-poetry.org | python3 -
export PATH="$HOME/.local/bin:$PATH"

# Install dependencies
poetry install

# Activate the virtual environment
poetry shell

# Ensure Jupyter is installed
poetry run pip install notebook

# Register Poetry environment in Jupyter
poetry run python -m ipykernel install --user --name=poetry-env --display-name "Python (Poetry)"

# Start Jupyter Notebook
poetry run jupyter notebook

```
This guide provides a structured approach to onboarding and running the obesity prediction analysis using Poetry and Jupyter Notebooks efficiently.
