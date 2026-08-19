# **ML Tabular Analysis** 📊

A hands-on collection of Jupyter notebooks for learning **tabular machine learning, data analysis, statistics, visualization, and core Python data-science tools**.

This repository is primarily a learning/reference project rather than a production ML system. It documents the progression from NumPy and pandas fundamentals to classification, ensemble learning, hyperparameter tuning, clustering, and visualization.

## 🚀 What This Repository Covers

### Machine Learning
- Classification models
  - Logistic Regression
  - K-Nearest Neighbors
  - Naive Bayes
  - Decision Trees
  - Support Vector Machines
- Ensemble learning
  - AdaBoost
  - Gradient Boosting
  - XGBoost
  - Stacking
- Hyperparameter optimization
  - GridSearchCV
  - RandomizedSearchCV
- Unsupervised learning
  - K-Means
  - DBSCAN
- Dimensionality reduction
  - PCA

### Data Science Foundations
- NumPy matrix operations
- Advanced NumPy/Python operations
- pandas data manipulation and analysis
- Statistics with Python
- Matplotlib and Seaborn visualization

### Python / CS Practice
- Linked-list implementation and practice

## 📁 Repository Structure

| Notebook | Main topic |
|---|---|
| `classificationmodels.ipynb` | Classification on the Titanic dataset |
| `Ensemblelearning.ipynb` | Stacking, AdaBoost, Gradient Boosting, XGBoost |
| `STACKING.ipynb` | Stacking classifier |
| `GridSearchcv (1).ipynb` | GridSearchCV and RandomizedSearchCV |
| `clusteringalgo.ipynb` | K-Means and DBSCAN |
| `PCA.ipynb` | Principal Component Analysis |
| `pandasfull.ipynb` | pandas practice and data manipulation |
| `pandas.ipynb` | pandas basics |
| `numpymatrixfunctions.ipynb` | NumPy matrix operations |
| `Copy of numpyadvpython.ipynb` | Advanced NumPy/Python practice |
| `statsinpy.ipynb` | Statistics in Python |
| `matplotlib.ipynb` | Data visualization |
| `linkedlist.ipynb` | Linked-list implementation |

> `.ipynb_checkpoints/` contains Jupyter's automatically generated checkpoint files and is not part of the learning path.

## 🧠 Learning Approach

The notebooks are intentionally practical: concepts are explored by loading datasets, inspecting data, preprocessing features, training models, and evaluating results.

Typical workflow:

1. Load and inspect the dataset
2. Handle missing values and categorical features
3. Split data into training and test sets
4. Apply preprocessing/scaling where appropriate
5. Train multiple ML algorithms
6. Compare model performance
7. Explore hyperparameter tuning or ensemble methods
8. Visualize results

## 🛠️ Tech Stack

- Python 3.7+
- Jupyter Notebook
- NumPy
- pandas
- scikit-learn
- Matplotlib
- Seaborn
- XGBoost

## ⚙️ Installation

Clone the repository and install the dependencies:

```bash
git clone https://github.com/krishna200822/ml-tabular-analysis.git
cd ml-tabular-analysis
pip install jupyter numpy pandas scikit-learn matplotlib seaborn xgboost
jupyter notebook
```

Then open the notebooks in Jupyter.

## 📊 Datasets

The notebooks mainly use small educational datasets, including:

- Titanic dataset from Seaborn
- Iris dataset from Seaborn
- Synthetic datasets generated with scikit-learn, including blobs and moons

These datasets are useful for understanding algorithms, but the repository does not yet demonstrate a complete real-world ML pipeline on a custom dataset.

## 🔍 Current Scope

This project focuses on **understanding and practicing ML concepts**, especially classical tabular ML.

It currently does **not** aim to provide:
- A production-ready ML pipeline
- Model deployment
- A frontend/backend application
- Experiment tracking
- Automated testing
- Reproducible environment management
- A polished end-to-end project with a business problem

Those would be natural next steps if the goal is to turn this learning repository into a portfolio-level ML project.

## 🧪 Important Improvements to Make

Before calling this production-quality, several things should be cleaned up:

- Use `fit_transform()` only on training data and `transform()` on test data.
- Put preprocessing and models inside `Pipeline` objects.
- Use cross-validation correctly and avoid tuning directly on the final test set.
- Report metrics beyond accuracy when appropriate.
- Add ROC-AUC / PR-AUC for binary classification where useful.
- Add confusion matrices and model comparison tables.
- Fix notebook typos and inconsistent variable names.
- Remove duplicated checkpoint files from version control.
- Add a `requirements.txt` or `pyproject.toml`.
- Add a clear project objective and dataset description.
- Add reproducible random seeds consistently.
- Separate exploratory notebooks from reusable Python modules.

## 📈 Project Status

**Status:** Learning / experimental ML repository

The repository demonstrates a solid foundation in classical tabular ML and data-science tooling, but it is still closer to a **structured learning portfolio** than a polished ML project.

## 👤 Author

**Krishna Sahu**

GitHub: `krishna200822`

## 📄 License

This repository is intended for educational use. Add an explicit open-source license if you want others to reuse, modify, and distribute the code under defined terms.

