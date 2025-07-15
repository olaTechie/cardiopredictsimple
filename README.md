# 🪀 Angina Risk Prediction App

A web-based clinical decision support tool to predict the risk of angina using patient-level features and a machine learning model.

## 🚀 Overview

This application uses a LightGBM model (developed with PyCaret) to predict whether a patient is at **high** or **low** risk of angina based on clinical, biochemical, and lifestyle parameters. It is built with [Streamlit](https://streamlit.io/) and offers an interactive sidebar for feature input and real-time prediction.

## 🔍 Key Features

- Interactive web app with patient-specific input fields
- Uses a pre-trained LightGBM classification model (`All_Variables_Model_LightGBM`)
- Displays real-time angina risk prediction
- Shows model feature importance plot
- Supports a wide range of clinical and laboratory variables

## 🧪 Input Features

The model accepts over 40 variables including:

- **Demographics**: Age, Sex, Ethnic Group
- **Vitals & Clinical History**: BMI, Blood Pressure, Chest Pain, Family History of CHD
- **Lifestyle Factors**: Smoking status, Physical activity
- **Lab Values**: HbA1c, Glucose, Lipids, Hemoglobin, Creatinine, etc.
- **Comorbidities**: Diabetes type, Hypertension treatment, Steroid use

## 📊 Output

The model returns a binary classification:

- ✅ **Low Risk** – Not predicted to have angina
- 🚨 **High Risk** – Predicted to have angina

## 🖼 Visuals

- Feature importance chart (`Preprocessed_model(important variables only) 2.png`)
- Sidebar input controls with default values
- Embedded ambulance image for UI branding

## 💠 How to Run

1. Clone this repo or download the code.
2. Ensure you have Python installed (preferably 3.8+).
3. Install the required packages:

```bash
pip install streamlit pandas pycaret pillow
```

4. Launch the app:

```bash
streamlit run predict_angina_app.py
```

## 📁 Files

- `predict_angina_app.py`: Streamlit app code
- `All_Variables_Model_LightGBM.pkl`: Pre-trained model (must be placed in same directory)
- `ambulance.jpg`: Sidebar branding image
- `Preprocessed_model(important variables only) 2.png`: Feature importance visualization

## 🧠 Model Info

- Framework: PyCaret
- Algorithm: LightGBM Classifier
- Input: Patient features as a single-row DataFrame
- Output: Binary prediction (0 = Low Risk, 1 = High Risk)

## 📌 Notes

- This tool is for **demonstration and research** purposes only.
- It is not intended for direct clinical use without further validation.

## 📬 Contact

For more information or collaboration inquiries, please contact:

**ALRUBAYYI ABDULAZIZ**  
[Abdulaziz.Alrubayyi@warwick.ac.uk](mailto:Abdulaziz.Alrubayyi@warwick.ac.uk)
