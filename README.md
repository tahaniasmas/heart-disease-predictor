# ❤️ Heart Disease Prediction System

##  Project Overview
This project aims to analyze and predict the presence of **heart disease** using **Business Intelligence and Machine Learning techniques**.  
By leveraging clinical patient data, the system assists in medical decision-making through accurate and interpretable predictions.

The project covers the **full data science lifecycle**, from data exploration and preprocessing to model evaluation and web deployment.

---

## Objectives
- Analyze and compare multiple heart disease datasets
- Preprocess clinical data for machine learning
- Train and evaluate several classification models
- Identify the most influential risk factors
- Deploy the best-performing model via a web interface

---

## Dataset
Two heart disease datasets were analyzed and compared:
- **Dataset 1**: 303 samples, 14 features, minimal missing values
- **Dataset 2**: 920 samples, 16 features, large number of missing values

➡️ **Dataset 1** was selected due to better data quality and usability.

---

## Data Preprocessing
The following preprocessing steps were applied:
- Removal of duplicate records
- Missing value imputation:
  - Median for numerical features
  - Mode for categorical features
- Encoding categorical variables using `LabelEncoder`
- Feature scaling using `StandardScaler`

---

## Machine Learning Models
The following models were trained and evaluated:
- Logistic Regression
- Random Forest
- XGBoost

### Model Performance Comparison

| Model               | Accuracy | Precision | Recall | F1-Score | ROC-AUC |
|--------------------|----------|-----------|--------|----------|---------|
| Logistic Regression | 0.82     | 0.82      | 0.82   | 0.82     | 0.93    |
| **Random Forest**   | **0.87** | **0.87**  | **0.87** | **0.87** | **0.94** |
| XGBoost            | 0.84     | 0.84      | 0.84   | 0.84     | 0.90    |

➡️ **Random Forest** was selected as the final model.

---

## Visualizations & Analysis
- Correlation matrix (heatmap)
- Feature importance analysis
- Confusion matrix
- ROC curve

These visualizations help interpret the model and identify key cardiovascular risk factors.

---

## Deployment
- **Framework**: Streamlit
- **Functionality**:
  - User inputs clinical parameters (age, cholesterol, chest pain type, etc.)
  - Model predicts presence or absence of heart disease instantly
- **Remote Access**:
  - Application exposed using **Ngrok**
  - Accessible via a secure public URL for real-time testing

---

## Technologies Used
- Python
- Scikit-learn
- XGBoost
- Pandas & NumPy
- Matplotlib & Seaborn
- Streamlit
- Ngrok

---

## How to Run the Project

```bash
pip install -r requirements.txt
streamlit run app.py
