# ❤️ Heart Disease Prediction App

A machine learning-powered web application that predicts the risk of heart disease based on patient clinical data. Built with **Scikit-learn**, **Python**, and deployed interactively using **Streamlit**.

---

## 📌 Project Overview

This project uses supervised machine learning to classify whether a patient is at risk of heart disease based on 13 clinical features such as age, cholesterol levels, chest pain type, resting ECG results, and more.

The model is served through an intuitive **Streamlit** web interface where healthcare professionals or researchers can input patient data and receive real-time predictions with confidence scores.

---

## 🚀 Demo

> Run locally or deploy via **Streamlit Cloud / Google Colab + ngrok**

![Heart Disease Prediction App]

<img width="347" height="665" alt="Screenshot 2026-04-15 104627" src="https://github.com/user-attachments/assets/90a268e6-d66e-459c-835f-f7db78121ae1" />

---

## 🧠 Features

- **13 Clinical Input Features** — age, sex, chest pain type, blood pressure, cholesterol, and more
- **Real-time Prediction** — instant risk classification (High Risk / No Risk)
- **Confidence Score** — probability output from the trained model
- **One-Hot Encoding** — handles categorical features like `thal` automatically
- **Preprocessing Pipeline** — standard scaling applied consistently to inputs
- **Clean UI** — built with Streamlit for zero-friction interaction

---

## 📂 Project Structure

```
heart-disease-prediction/
│
├── Heart_Disease.ipynb                     # Model training & EDA notebook
├── streamlit_heartdiseaseprediction.py     # Streamlit app source
├── heart_model.pkl                         # Trained ML model
├── scaler.pkl                              # StandardScaler for input normalization
├── model_columns.pkl                      # Column structure for consistent encoding
└── LICENSE
└── README.md
```

---

## 🔬 Input Features

| Feature | Description |
|---|---|
| `slope_of_peak_exercise_st_segment` | Slope of peak exercise ST segment (0–2) |
| `thal` | Thalassemia (`normal`, `reversible_defect`, `fixed_defect`) |
| `resting_blood_pressure` | Resting blood pressure (mm Hg) |
| `chest_pain_type` | Type of chest pain (0–3) |
| `num_major_vessels` | Number of major vessels colored by fluoroscopy (0–3) |
| `fasting_blood_sugar_gt_120_mg_per_dl` | Fasting blood sugar > 120 mg/dl (1 = True) |
| `resting_ekg_results` | Resting ECG results (0–2) |
| `serum_cholesterol_mg_per_dl` | Serum cholesterol (mg/dl) |
| `oldpeak_eq_st_depression` | ST depression induced by exercise (float) |
| `sex` | Sex (0 = Female, 1 = Male) |
| `age` | Age of the patient (years) |
| `max_heart_rate_achieved` | Maximum heart rate achieved |
| `exercise_induced_angina` | Exercise-induced angina (0 = No, 1 = Yes) |


---

## 🏗️ Model Training

The model was trained in `Heart_Disease.ipynb`. The pipeline includes:

1. **Exploratory Data Analysis (EDA)** — distributions, correlations, class balance
2. **Preprocessing** — one-hot encoding for categorical features, `StandardScaler` for numerical features
3. **Model Training** — classification model (e.g., Logistic Regression / Random Forest)
4. **Evaluation** — accuracy, precision, recall, F1-score, confusion matrix
5. **Serialization** — model, scaler, and column structure saved using `pickle`

---

## 📊 Model Artifacts

| File | Description |
|---|---|
| `heart_model.pkl` | Trained classification model |
| `scaler.pkl` | Fitted `StandardScaler` for input normalization |
| `model_columns.pkl` | Expected column order after one-hot encoding |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.x | Core language |
| Scikit-learn | ML model training & preprocessing |
| Pandas / NumPy | Data manipulation |
| Streamlit | Web app framework |
| Pickle | Model serialization |
| Google Colab | Training environment |
| ngrok / pyngrok | Tunneling for Colab deployment |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author

**MOKSHA VAINAVI S**  

---

> ⚠️ **Disclaimer:** This tool is intended for educational and research purposes only. It is not a substitute for professional medical diagnosis or advice.
