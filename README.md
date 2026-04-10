# Assignment-10
Assignment 10 AI course 

# Amazon Alexa Sentiment Analysis

## Project Overview
This project focuses on performing sentiment analysis on Amazon Alexa customer reviews. The goal is to classify reviews as either **positive or negative** using machine learning techniques.

The dataset contains customer feedback, product variation, ratings, and textual reviews. We use Natural Language Processing (NLP) and a **Random Forest Classifier** to build the model.

---

## Objective
To build a machine learning model that can:
- Analyze customer reviews
- Convert text data into numerical format
- Predict sentiment (Positive or Negative)
- Evaluate model performance using classification metrics

---

## Dataset Description
The dataset includes:
- `verified_reviews` → Customer review text
- `rating` → Product rating
- `variation` → Product type
- `feedback` → Target variable (1 = Positive, 0 = Negative)

Source: Amazon Alexa product review dataset (Kaggle / public dataset)

---

## Technologies Used
- Python 
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

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
