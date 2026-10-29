
# Credit Card Fraud Detection Using Machine Learning

## Project Overview
This project uses machine learning to classify credit card transactions as legitimate or potentially fraudulent.

It uses Python, Pandas and Scikit-learn to explore transaction data, train classification models, and evaluate their ability to detect fraud.

## Objectives
- Explore and understand transaction data.
- Investigate the imbalance between legitimate and fraudulent transactions.
- Train and compare Logistic Regression and Random Forest.
- Evaluate results using precision, recall, F1-score and Average Precision.

## Technologies Used
- Python 3.11
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Joblib
- JupyterLab

## Dataset
Credit Card Fraud Detection dataset.

Source:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

The dataset contains anonymised transaction features and a `Class` target column:
- `0` = Legitimate transaction
- `1` = Fraudulent transaction

The dataset is not included in this repository. Download it separately and place `creditcard.csv` inside the `data/` folder.

## Project Workflow
1. Load and inspect the dataset.
2. Explore missing values, duplicates and class distribution.
3. Split the data into training, validation and testing sets.
4. Train Logistic Regression and Random Forest models.
5. Select a model using validation Average Precision.
6. Evaluate the selected model on held-out test data.
7. Save the trained model locally.

## Test Results
Selected model: Random Forest

Results from the current run:
- Fraud precision: 0.9615
- Fraud recall: 0.7653
- Fraud F1-score: 0.8523
- Test Average Precision: 0.8513
- Overall accuracy: approximately 99.95%

Confusion matrix:
- True negatives: 56,861
- False positives: 3
- False negatives: 23
- True positives: 75

These are results from one train-validation-test split and may vary with changes to the experiment.

## How to Run the Project

1. Clone or download this repository.
2. Download the dataset from the source linked above.
3. Create a `data/` folder in the project directory.
4. Place `creditcard.csv` inside the `data/` folder.
5. Install the required Python packages:

   `pip install -r requirements.txt`

6. Start JupyterLab:

   `jupyter lab`

7. Open `credit_card_fraud_detection.ipynb` and run the cells from top to bottom.

## Limitations
This is an educational machine learning project using historical, anonymised data. It is not a production banking fraud detection system, and its predictions should not be used to make real payment decisions.

## Author
Samruddhi More
MCA Student | Interested in Data Science and Machine Learning
