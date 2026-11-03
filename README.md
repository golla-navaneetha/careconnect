# CareConnect – Patient Appointment Management and No-Show Prediction

## Project Overview

CareConnect is a patient appointment management project that combines a Streamlit application with a Machine Learning model to predict the likelihood of patients missing scheduled medical appointments. By identifying patients who are likely to be no-shows, clinics can plan better, send timely reminders, and reduce wasted appointment slots.

## Features

- Patient appointment information management
- Machine Learning-based appointment no-show prediction
- Data preprocessing and feature engineering
- Interactive Streamlit interface
- Prediction using a trained Random Forest classifier

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Joblib

## Project Structure

```
careconnect/
├── app.py                  # Streamlit application
├── train_model.py          # Machine Learning model training
├── careconnect_model.pkl   # Saved trained model
├── requirements.txt        # Project dependencies
├── .gitignore
└── README.md
```

## How to Run Locally

1. **Clone this repository**

   ```bash
   git clone https://github.com/golla-navaneetha/careconnect.git
   cd careconnect
   ```

2. **Install the required dependencies**

   ```bash
   pip install -r requirements.txt
   ```

3. **Train the model** (skip if `careconnect_model.pkl` already exists)

   ```bash
   python train_model.py
   ```

4. **Run the application**

   ```bash
   streamlit run app.py
   ```

   The app opens in your browser at `http://localhost:8501`.

## How It Works

1. Appointment and patient details are entered in the Streamlit interface.
2. The data is preprocessed and converted into the features the model expects.
3. The trained Random Forest classifier predicts whether the patient is likely to attend or miss the appointment.
4. The result is displayed on the page.

## Project Status

Ongoing – Application and Machine Learning components are under development.

## Author

**Golla Navaneetha**
GitHub: [@golla-navaneetha](https://github.com/golla-navaneetha)
