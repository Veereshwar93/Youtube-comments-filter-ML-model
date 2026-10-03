# Youtube-comments-filter-ML-model

## Overview

This project uses machine learning to classify YouTube comments as **Spam** or **Not Spam**.

The project applies text preprocessing and TF-IDF vectorization before training and comparing multiple machine-learning classification models.

## Project Workflow

```text
YouTube Comments
       ↓
Data Preprocessing
       ↓
Train/Test Split
       ↓
TF-IDF Vectorization
       ↓
Train Multiple ML Models
       ↓
Model Evaluation
       ↓
Random Forest Model
       ↓
New Comment Prediction
```

## Models Used

The project trains and compares:

- Logistic Regression
- Support Vector Classifier (SVC)
- Random Forest
- Naive Bayes
- XGBoost

The models are evaluated using metrics such as:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC

## Final Prediction

After comparing the models, the project uses the saved Random Forest model for testing new, unseen comments.

New comments are first transformed using the trained TF-IDF vectorizer and then passed to the Random Forest classifier.

Example:

```text
New YouTube Comment
        ↓
TF-IDF Vectorization
        ↓
Random Forest
        ↓
Spam / Not Spam
```

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn
- Joblib
- Google Colab

## How to Run

1. Clone the repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Run the cells in order.

The notebook contains the complete data preprocessing, model training, evaluation, and manual testing workflow.

## Project Files

| File | Description |
|---|---|
| `youtube_comment_filter_ML_project.ipynb` | Complete machine-learning notebook |
| `models/RFC_model.pkl` | Trained Random Forest model |
| `models/tfidf_vectorizer.pkl` | Saved TF-IDF vectorizer |
| `requirements.txt` | Required Python libraries |
| `dataset/` | Dataset information |

## Key Learning

Through this project, I learned how to build a text-classification pipeline, convert text into numerical features using TF-IDF, train and compare multiple machine-learning models, evaluate their performance, and use a trained model to classify new comments.
