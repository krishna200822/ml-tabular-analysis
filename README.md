🧠 ML Practice Projects

This repo is basically me trying to actually understand machine learning instead of just watching videos and pretending I get it.

Right now it has two small projects where I went step by step from raw data → cleaning → feature engineering → model → evaluation.

Nothing fancy. Just real practice.

---

📁 Projects

1. Insurance Cost Prediction

In this project, I worked with a dataset that includes age, BMI, smoking habits, etc., and tried to predict insurance charges.

What I actually did:

- Checked the data properly instead of blindly training
- Looked at distributions and outliers (boxplots, histograms)
- Converted categorical data into numbers
- Created some extra features (like BMI categories)
- Scaled features
- Trained a Linear Regression model

Result:

- R² score came around 0.79

Not perfect, but decent for a basic model.

File:

- "insuranceproject.ipynb"

---

2. Heart Disease Prediction

This one is a classification problem where the goal is to predict if a person has heart disease.

What I did here:

- Explored the dataset (counts, distributions, relationships)
- Found some weird values (like cholesterol = 0) and fixed them
- Used encoding for categorical features
- Checked correlations
- Applied feature scaling

Some observations:

- Features like max heart rate and oldpeak seem pretty important
- Certain categories (like chest pain type) clearly affect the output

File:

- "Heart.ipynb"

---

⚙️ Tools I Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

---

🚀 How to Run

Clone the repo:

git clone https://github.com/krishna200822/Insurance-anayzler-for-model.git

Install dependencies:

pip install numpy pandas matplotlib seaborn scikit-learn

Open the notebooks and run them step by step.

---

📌 What I’m Trying to Learn

- How data actually behaves (not just theory)
- When and why to clean or transform data
- How features affect model performance
- How to move from intuition → implementation

---

⚠️ Honest Note

This is not an advanced project.

I’m still learning:

- Better models
- Proper validation
- Avoiding mistakes like data leakage
- Writing cleaner pipelines

This repo is just part of that process.

---
🚗 Ford Car Price Prediction
📌 Problem Statement

The objective of this project is to predict the price of used Ford cars using structured tabular data. The dataset includes multiple features such as model type, mileage, fuel type, transmission, and engine size, which influence the car price.

📊 Dataset
Source: Kaggle Ford Car Dataset
Shape: 17,966 rows × 9 columns
Features:
model (categorical)
year (numerical)
price (target variable)
transmission (categorical)
mileage (numerical)
fuelType (categorical)
tax (numerical)
mpg (numerical)
engineSize (numerical)

✔ No missing values in dataset

🔍 Exploratory Data Analysis (EDA)
Analyzed distribution of price using histogram
Observed spread and skewness in car prices
Summary statistics:
Mean price ≈ 12,279
Wide range from very low to high-end vehicles
Key Observations:
Mileage shows negative relationship with price
Newer cars tend to have higher prices
Engine size and fuel efficiency influence price moderately
⚙️ Data Preprocessing
Checked dataset structure using .info()
Verified no null values
Separated features (X) and target (y)
Applied encoding techniques:
Label Encoding for categorical variables
One-Hot Encoding (for comparison experiment)
Feature scaling applied to numerical features
🧪 Experiment: Encoding Comparison

Two encoding techniques were tested to evaluate their effect on model performance:

1. Label Encoding
Converts categories into integer values
Introduces ordinal relationship (not always correct)
2. One-Hot Encoding
Creates binary columns for each category
Preserves independence of categories
🤖 Model Training
Algorithm: Linear Regression
Train-Test Split: 80-20
Model trained on processed dataset
🧠 Key Insights
Encoding choice significantly affects model performance
One-Hot Encoding performs better as it avoids false ordinal relationships
Linear Regression provides a baseline but may not capture complex patterns
⚠️ Limitations
Linear model cannot capture non-linear relationships
Label Encoding introduces misleading numerical ordering
No advanced feature engineering applied
🚀 Future Improvements
Use advanced models:
Random Forest
XGBoost
Perform feature engineering
Hyperparameter tuning
Cross-validation

👤 Author

Krishna
Trying to get good at ML by actually doing the work instead of skipping steps
