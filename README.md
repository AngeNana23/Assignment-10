# Assignment-10
Assignment 10 AI course 

Amazon Alexa Sentiment Analysis
Project Overview
This project performs sentiment analysis on Amazon Alexa customer reviews using machine learning. The objective is to classify reviews as positive or negative based on their textual content.
A Random Forest Classifier is used as the main model, with Logistic Regression included for comparison. Text data is converted into numerical form using Count Vectorization.
Dataset
File: amazon_alexa.tsv
Features include:
verified_reviews (text data)
variation (product type)
feedback (target variable)
Target Labels:
1 → Positive review
0 → Negative review
Technologies Used
Python
Google Colab
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
Methodology
Data Preprocessing
Removed unnecessary columns (date, rating)
Handled missing values
One-hot encoded the variation column
Converted text into numerical features using CountVectorizer
Model Training
Split dataset into 80% training and 20% testing
Trained:
Random Forest Classifier
Logistic Regression (baseline model)
Evaluation
Confusion Matrix
Classification Report (Precision, Recall, F1-score)
ROC Curve and AUC score
Results
Accuracy: approximately 93%
AUC Score: approximately 0.91
Key Findings:
Strong performance on positive reviews
Lower performance on negative reviews due to class imbalance
Important features include words such as “not”, “back”, “stopped”, and “terrible”

---

## Workflow

### 1. Data Preprocessing
- Handled missing values
- Dropped irrelevant columns (`date`, `rating`)
- One-hot encoded categorical variables (`variation`)

### 2. Feature Engineering
- Applied **CountVectorizer** to convert text into numerical features
- Combined text features with structured data

### 3. Model Building
- Random Forest Classifier (100 estimators)
- Train-test split (80/20)

### 4. Model Evaluation
- Confusion Matrix
- Classification Report
- Accuracy Score

---

## Model Performance
The model was evaluated using:

- Accuracy
- Precision
- Recall
- F1-score

The Random Forest model performed well in classifying customer sentiment.

---

## Results Visualization
The project includes:
- Feedback distribution plots
- Variation vs rating analysis
- Confusion matrix heatmap
- Feature importance graph

---

## How to Run the Project

1. Open Google Colab
2. Mount Google Drive
3. Load dataset (`amazon_alexa.tsv`)
4. Run all notebook cells sequentially
5. View results and visualizations

---

## Installation Requirements
If running locally:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
