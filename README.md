# 🎬 KNN Model Performance Analysis and Hyperparameter Optimization for Movie Analytics

## 📌 Project Overview

This project focuses on analyzing and improving the performance of a **K-Nearest Neighbor (KNN)** machine learning model for movie classification based on movie characteristics and audience ratings.

The movie industry produces large amounts of data such as production budget, revenue, popularity, runtime, and audience ratings. This data can be analyzed to discover patterns and classify movies based on their performance.

In this project, the KNN model is evaluated using several evaluation metrics and optimized through **Hyperparameter Tuning using GridSearchCV** to find the best parameter combination and improve classification performance.

---

# 🎯 Objectives

The objectives of this project are:

- Analyze movie characteristics based on available features:
  - Budget
  - Revenue
  - Popularity
  - Runtime
  - Rating

- Build a **K-Nearest Neighbor (KNN)** classification model to categorize movies based on rating.

- Evaluate model performance using:
  - Accuracy
  - Precision
  - Recall
  - F1-Score
  - ROC-AUC

- Perform **Hyperparameter Tuning using GridSearchCV** to find the optimal KNN parameters.

- Compare model performance before and after hyperparameter optimization.

---

# 📊 Dataset

The dataset used in this project is obtained from **Kaggle** and consists of:

- `movies_metadata.csv`
- `ratings_small.csv`

The dataset contains movie information and audience ratings that are used for analysis and classification.

## Features Used

| Feature | Description |
|---|---|
| id | Unique identifier for each movie |
| budget | Movie production cost |
| revenue | Total movie revenue |
| runtime | Movie duration |
| popularity | Movie popularity score |
| vote_average | Average audience rating |
| release_date | Movie release date |
| original_language | Original movie language |
| rating | Audience rating category |

---

# 🛠 Tools & Technologies

## Development Environment

- Google Colab

## Programming Language

- Python

## Python Libraries

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

The tools are used for:
- Data preparation
- Data processing
- Machine learning model development
- Model evaluation
- Hyperparameter optimization

---

# 🔄 Project Workflow

The workflow of this project:

```
Dataset
   ↓
Data Preparation
   ↓
Data Cleaning
   ↓
Feature Selection
   ↓
KNN Model Development
   ↓
Model Evaluation
   ↓
Hyperparameter Tuning
   ↓
Performance Analysis
   ↓
Conclusion
```

## Workflow Explanation

### 1. Data Preparation
- Import movie datasets.
- Clean and process data.
- Combine required datasets.
- Select relevant features.

### 2. Model Development
- Build KNN classification model.
- Train the model using movie characteristics.

### 3. Model Evaluation & Optimization
- Evaluate model performance.
- Optimize parameters using GridSearchCV.
- Compare results before and after tuning.

---

# 🤖 Machine Learning Model

## K-Nearest Neighbor (KNN)

KNN is a supervised machine learning algorithm used for classification by finding similarities between data points.

In this project, KNN is used to classify movies based on patterns from movie features.

## Initial Model Parameters

```
n_neighbors = 5
p = 2
metric = minkowski
```

After testing different configurations, the model was adjusted using:

```
n_neighbors = 7
p = 1
```

The model then learned patterns from the training dataset and was used for prediction.

---

# ⚙️ Hyperparameter Optimization

## GridSearchCV

Hyperparameter tuning was performed using **GridSearchCV** to find the best combination of KNN parameters.

The best parameters obtained:

```
n_neighbors = 3
p = 1
```

These parameters were selected because they produced better classification performance compared to the initial configuration.

---

# 📈 Model Evaluation

The model was evaluated using several performance metrics:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

## Performance Before Optimization

| Metric | Score |
|---|---|
| Accuracy | 83% |
| Precision | 85% |
| Recall | 97% |
| F1-Score | 91% |

The evaluation shows that the model was able to recognize positive movie categories effectively, but still had difficulty identifying minority classes.

---

# 📊 Performance After Optimization

After applying hyperparameter tuning, the model achieved:

| Metric | Score |
|---|---|
| Accuracy | 85.7% |
| Precision | 85.7% |
| Recall | 100% |
| F1-Score | 92.3% |

The optimization process improved the overall classification performance of the KNN model.

---

# 💡 Key Insights

- KNN can be used to classify movie categories based on available movie characteristics.
- Features such as **budget, popularity, and vote average** provide important information for classification.
- Hyperparameter tuning using GridSearchCV improves model performance.
- Selecting appropriate parameters has a significant impact on prediction results.
- Model evaluation should use multiple metrics to provide a more complete performance analysis.
- The model still has limitations and can be improved with additional features or different machine learning algorithms.

---

# 🚀 Recommendations

Future improvements that can be implemented:

1. Add additional movie features:
   - Genre
   - Number of votes
   - Director
   - Actor information

2. Perform further hyperparameter optimization.

3. Use a more balanced dataset distribution to reduce prediction bias.

4. Compare KNN performance with other machine learning algorithms:
   - Decision Tree
   - Random Forest
   - Support Vector Machine

5. Evaluate and update the model periodically when new movie data becomes available.

---

# 🏁 Conclusion

This project demonstrates the implementation of the **K-Nearest Neighbor (KNN)** algorithm for movie classification based on audience ratings.

Model evaluation provides insights into prediction performance, while **Hyperparameter Tuning using GridSearchCV** helps identify better parameter configurations to improve model accuracy.

Through optimization and evaluation, the model can provide better classification results and deeper analytical insights into movie data.

