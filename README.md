# COVID-19 Death Prediction Using Machine Learning

This project focuses on building a machine learning model to predict the likelihood of death in COVID-19 patients based on clinical and demographic features. The dataset is sourced from Kaggle and contains real-world patient information such as age, comorbidities, ICU admission, and more.

## 🔍 Objective

To predict whether a COVID-19 patient will survive or die based on key medical features, using classification algorithms and feature engineering techniques.

---

## 📁 Dataset

- **Source**: [Kaggle - COVID-19 Dataset](https://www.kaggle.com/datasets/meirnizri/covid19-dataset)
- **Filename**: `Covid Data.csv`
- **Rows**: 5+ million records
- **Columns**:
  - USMER, MEDICAL_UNIT, SEX, PATIENT_TYPE, DATE_DIED, INTUBED, PNEUMONIA, AGE, PREGNANT, DIABETES, COPD, ASTHMA, INMSUPR, HIPERTENSION, OTHER_DISEASE, CARDIOVASCULAR, OBESITY, RENAL_CHRONIC, TOBACCO, CLASIFFICATION_FINAL, ICU

---

## 🧹 Data Cleaning

- Removed invalid or placeholder values (e.g., 97, 98, 99).
- Encoded target variable `DATE_DIED` as:
  - **1** for death (i.e., valid date)
  - **0** for alive (i.e., '9999-99-99')
- Converted categorical variables to numeric using Label Encoding.
- Removed or imputed missing values in features like `INTUBED`, `ICU`, etc.

---

## 🎯 Target Variable

- **Target**: `Death`
  - `1`: Patient died
  - `2`: Patient survived

---

## 🛠️ Features Used

Selected features for training:

- AGE
- SEX
- PNEUMONIA
- DIABETES
- COPD
- ASTHMA
- INMSUPR (Immunosuppression)
- HIPERTENSION
- CARDIOVASCULAR
- OBESITY
- RENAL_CHRONIC
- TOBACCO
- INTUBED
- ICU

---

## 🤖 Models Applied

- Logistic Regression
- Random Forest Classifier
- XGBoost
- Support Vector Machine

---

## 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Score

---

## 📌 Key Takeaways

- `AGE`, `ICU`, `INTUBED`, and `DIABETES` are major predictors of mortality.
- XGBoost outperformed other models with highest accuracy.
- Proper preprocessing and handling of missing/invalid values significantly boosted performance.

---

## 🧠 Future Improvements

- Use deep learning models for better predictions.
- Apply SHAP or LIME for explainability.
- Deploy model with a web app interface using Flask or Streamlit.

---

## 📚 License

This project is licensed under the MIT License.

---

## 👩‍💻 Author

**Sobia Noor**  
Data Scientist | AI & ML Enthusiast  
[GitHub](https://github.com/SobiaNoorAI) | [LinkedIn](https://www.linkedin.com/in/sobianoorai/)
