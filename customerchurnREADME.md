# Customer Churn Prediction using Deep Learning

This project aims to predict customer churn in a telecommunications company using a deep learning model built with TensorFlow and Keras. It includes steps like data preprocessing, model training, evaluation, and performance visualization.

---

## Dataset

The dataset used is **Telco Customer Churn**, from Kaggle. It contains customer details such as services subscribed, account information, demographics, and whether or not they have churned.  
LINK : https://www.kaggle.com/datasets/blastchar/telco-customer-churn

> The dataset is provided in a ZIP format: `telco churn.zip`  
> Inside it: `WA_Fn-UseC_-Telco-Customer-Churn.csv`

---

## Project Workflow

### 1. Import Libraries
All essential Python libraries are imported for data manipulation, visualization, machine learning, and deep learning.

### 2. Data Extraction
The ZIP file is extracted to access the CSV file.

### 3. Data Cleaning & Preprocessing
- Dropping irrelevant columns (`customerID`)
- Handling missing or non-numeric values (`TotalCharges`)
- One-hot encoding of categorical features
- Feature scaling using `StandardScaler`

### 4. Model Building
- Built a simple neural network using Keras:
  - Input Layer → Hidden Layers → Output Layer
  - `ReLU` activation for hidden layers, `sigmoid` for output
- Compiled with `adam` optimizer and `binary_crossentropy` loss
- Trained using `fit()` for 50 epochs

### 5. Model Evaluation
- Predictions on test data
- Confusion Matrix using Seaborn
- Classification Report (Precision, Recall, F1-Score)
- ROC Curve & AUC Score

---

## Tools & Libraries Used

- Python 3.x
- Pandas / NumPy
- Seaborn / Matplotlib
- scikit-learn
- TensorFlow / Keras

---

## How to Run

1. Clone this repo or upload the notebook to Google Colab.
2. Upload the dataset zip file `telco churn.zip`.
3. Run the notebook cells in order.

---

## Output

- Confusion Matrix Heatmap
- Precision, Recall, F1-score
- ROC Curve with AUC Score
