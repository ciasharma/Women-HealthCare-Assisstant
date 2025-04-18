
# 👩 Women's Health Assistant

A one-stop solution for PCOS prediction, period tracking, diet planning, and image-based PCOS detection using Streamlit.

---

## 🚀 Features

### 🩺 PCOS Detection (Tab 2)
Predict PCOS based on health and physiological data using a pre-trained machine learning model.

**Inputs Include:**
- Age, Weight, Height, BMI
- Blood Group, Pulse Rate, Respiratory Rate
- Hemoglobin, Cycle Regularity, Cycle Length
- Marital Status, Pregnancy, Abortions
- Waist-Hip Measurements & Ratio
- Symptoms: Weight Gain, Hair Growth, Skin Darkening, Hair Loss, Pimples, Fast Food, Exercise
- Blood Pressure

**Model:** `data_model.pkl` (loaded via `joblib`)

---

### 📅 Period Tracker (Tab 3)
Predict the next period date by entering the last period start date and average cycle length.

**Features:**
- Auto-calculates the next period date using datetime operations.

---

### 🥗 Diet Plan (Tab 4)
Provides a PCOS-friendly diet plan based on user's weight, activity level, and diet preference.

**Macronutrient Calculation Logic:**
- 30% Protein, 40% Carbohydrates, 30% Fats
- Example meals include oats, nuts, grilled proteins, and lentils.

---

### 🖼️ Image-based PCOS Detection (Tab 5)
Upload an ultrasound image to detect signs of PCOS using a deep learning image model.

**Model:** `image_model.keras` (TensorFlow Keras model)

**Image Preprocessing:**
- Resize to (224x224)
- Normalize pixel values
- Predict using the model and show result

---

## 🛠 Technologies Used

- **Streamlit** – Web application interface
- **scikit-learn** – PCOS prediction model (`joblib`)
- **TensorFlow/Keras** – Deep learning model for image-based diagnosis
- **NumPy** – Data manipulation
- **PIL / Keras Image Preprocessing** – Image input handling
- **datetime** – For period tracking

---

## 📂 Files Required

- `data_model.pkl` – ML model for tabular PCOS prediction
- `image_model.keras` – CNN model for ultrasound-based PCOS detection
- Optional: `home.jpg` for the home tab visual

---

## 🧪 How to Run

```bash
streamlit run your_script_name.py
```

Ensure all required models and images are in the same directory or provide full paths.

---

## 📌 Notes

- Image-based detection assumes proper ultrasound input
- Predictions are based on trained model data and may not replace professional medical advice

---

## 📷 Example Ultrasound Upload Prediction

- Upload: `.jpg`, `.jpeg`, `.png`
- Result: PCOS Detected or Not Detected based on model inference

---

## ❤️ Designed For
Women's health awareness, diagnosis assistance, and health tracking in an easy-to-use platform.
