# 🧠 ML Tabular Analysis - Learning by Doing

A collection of machine learning projects focused on tabular data analysis. This repository documents my journey in understanding ML fundamentals through hands-on implementation rather than just theory.

**Philosophy**: Raw data → EDA → Cleaning → Feature Engineering → Modeling → Evaluation

---

## 📁 Projects Overview

### 1. 🏥 Heart Disease Prediction
**Type**: Classification Problem  
**Objective**: Predict whether a patient has heart disease based on medical indicators

**Dataset**:
- **File**: `heart.csv`
- **Samples**: 918 records
- **Features**: 11 medical indicators + 1 target variable
- **Target**: HeartDisease (Binary: 0 or 1)

**Key Features**:
- Age, Sex, Chest Pain Type
- Resting Blood Pressure, Cholesterol
- Fasting Blood Sugar, Resting ECG
- Max Heart Rate, Exercise Angina
- Oldpeak (ST depression), ST Slope

**What I Did**:
- ✅ Explored distributions and identified data quality issues
- ✅ Fixed anomalies (cholesterol = 0, resting BP = 0) using mean imputation
- ✅ Performed categorical encoding (one-hot encoding)
- ✅ Analyzed correlations with target variable
- ✅ Applied feature scaling for numerical features
- ✅ Visualized relationships using countplots, boxplots, violin plots, and heatmaps

**Key Findings**:
- 55.3% of patients have heart disease in the dataset
- Max Heart Rate shows strong inverse relationship with disease
- Oldpeak (ST depression) is a significant indicator
- Chest pain type significantly affects prediction
- Features like Sex and Exercise Angina are important discriminators

**Notebook**: `Heart.ipynb`

---

### 2. 💰 Insurance Cost Prediction
**Type**: Regression Problem  
**Objective**: Predict medical insurance charges based on demographic and lifestyle factors

**Dataset**:
- **File**: `insurance.csv`
- **Target**: Insurance charges (continuous variable)

**What I Did**:
- Analyzed distribution of insurance charges
- Handled categorical features (region, smoking status)
- Created feature engineering:
  - BMI categories (Underweight, Normal, Overweight, Obese)
  - Age groups
- Applied One-Hot Encoding for categorical variables
- Normalized/scaled numerical features
- Trained Linear Regression model
- Evaluated using R² score and other metrics

**Model Performance**:
- **R² Score**: ~0.79
- **Interpretation**: Model explains ~79% of variance in insurance costs

**Insights**:
- Smoking status is the strongest predictor of insurance charges
- Age and BMI are significant factors
- Geographic region has a moderate impact
- Positive correlation between age and charges

**Notebook**: `insuranceproject.ipynb`

---

### 3. 🚗 Ford Car Price Prediction
**Type**: Regression Problem  
**Objective**: Predict used Ford car prices from tabular features

**Dataset**:
- **File**: `ford.csv`
- **Samples**: 17,966 records
- **Target**: Price (continuous variable)

**Features**:
| Feature | Type | Description |
|---------|------|-------------|
| Model | Categorical | Car model type |
| Year | Numerical | Manufacturing year |
| Transmission | Categorical | Manual/Automatic |
| Mileage | Numerical | Miles driven |
| Fuel Type | Categorical | Petrol/Diesel/Hybrid |
| Tax | Numerical | Annual tax |
| MPG | Numerical | Miles per gallon |
| Engine Size | Numerical | Engine displacement |

**What I Did**:
- ✅ EDA: Analyzed price distribution and feature relationships
- ✅ Data Quality: Verified no missing values
- ✅ Categorical Encoding Comparison:
  - **Label Encoding**: Converts to integers (introduces false ordering)
  - **One-Hot Encoding**: Creates binary columns (preserves independence)
- ✅ Feature Scaling: Applied to numerical features
- ✅ Model Training: Linear Regression baseline
- ✅ Performance Comparison: Evaluated both encoding methods

**Key Observations**:
- Newer cars command higher prices
- Strong negative correlation between mileage and price
- Engine size and fuel efficiency (MPG) moderately influence price
- **One-Hot Encoding outperforms Label Encoding** (avoids misleading ordinal relationships)

**Experiment Results**:
- One-Hot Encoding showed better model performance
- Demonstrated importance of proper categorical variable handling

**Limitations & Future Work**:
- ⚠️ Linear model cannot capture non-linear patterns
- 🚀 Upgrade to Random Forest, XGBoost for better performance
- 🚀 Implement feature engineering (price per year, efficiency ratios)
- 🚀 Add hyperparameter tuning and cross-validation
- 🚀 Explore interaction effects

**Notebook**: `fordcar.ipynb`

---

## 📚 Additional Learning Materials

This repo also includes foundational learning notebooks:
- `numpyadvpython.ipynb` - NumPy advanced operations
- `numpymatrixfunctions.ipynb` - Matrix manipulations
- `pandasfull.ipynb` - Comprehensive Pandas tutorial
- `pandas.ipynb` - Basic Pandas operations
- `logticregression1.ipynb` - Logistic Regression deep dive
- `statsinpy.ipynb` - Statistical concepts in Python
- `linkedlist.ipynb` - Data structures

---

## 🛠️ Tech Stack

**Languages & Libraries**:
- Python 3.12+
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Analysis**: sheryanalysis (custom package)

---

## ⚙️ Installation & Setup

**Clone the repository**:
```bash
git clone https://github.com/krishna200822/ml-tabular-analysis.git
cd ml-tabular-analysis






