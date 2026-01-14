
# Arogya-AI

Arogya-AI is a **smart, offline-first healthcare assistance web application** designed to support symptom checking, risk prediction, and Primary Health Center (PHC) workflows using AI-inspired logic, Firebase, and a modern React UI.

---

## ✨ Key Features

- 🩺 **Pocket Doctor – Symptom Checker**
  - Structured symptom selection
  - Free-text symptom notes
  - Real-time vitals validation (BP, SpO₂, sugar, temperature)

- 🧠 **Offline AI Risk Prediction**
  - Simulated TFLite-style ML model
  - Uses age, vitals, lab values, and symptom severity
  - Outputs Low / Moderate / High Risk instantly (no internet needed)

- 🚨 **Clinical Triage & Alerts**
  - Detects critical vitals automatically
  - Prevents report submission if emergency values are found

- 🧪 **Lab Report Simulation**
  - Upload/simulate lab results (Normal / Warning / High Risk)

- 🏥 **PHC Dashboard**
  - Real-time patient reports via Firebase Firestore
  - Filter by:
    - Critical cases
    - Prescribed / Unprescribed
  - Search by name, address, or patient ID

- 🧾 **Doctor Prescription System**
  - View patient history
  - Write prescriptions, diet advice, and notes
  - Saved securely to Firestore with timestamps

- 📊 **Offline Risk Trend Visualization**
  - Simple health-risk trend chart using Recharts

---

## 🛠 Tech Stack

- **Frontend:** React, Tailwind CSS
- **Backend:** Firebase (Auth + Firestore)
- **Charts:** Recharts
- **Icons:** lucide-react
- **Auth:** Anonymous / Custom Token Firebase Auth
- **AI Logic:** Rule-based + ML-inspired risk scoring (offline)

---

## 📥 Input Parameters (AI Model)

The simulated AI model uses **10 inputs**:

| Index | Parameter |
|-----|-----------|
| 0 | Age |
| 1 | Gender |
| 2 | Systolic BP |
| 3 | Fasting Sugar |
| 4 | Body Temperature |
| 5 | SpO₂ |
| 6 | Symptom Severity |
| 7 | Structured Symptom Score |
| 8 | HbA1c |
| 9 | Cholesterol |

---

## 🔐 Firebase Configuration

Firebase config is injected via environment variables:

- `__firebase_config`
- `__app_id`
- `__initial_auth_token`

Authentication falls back to **anonymous login** if no token is provided.

---

## ▶️ Running the Project

```bash
npm install
npm start
````

---

## ⚠️ Medical Disclaimer

This application **does not replace professional medical advice**.
All recommendations are preliminary and for educational/demo purposes only.
Always consult a certified healthcare professional for diagnosis and treatment.

---

## 📄 License

This project is intended for **academic, demo, and research purposes**.

---

## 🙏 Acknowledgements

Built to support **digital healthcare access**, **offline AI**, and **PHC efficiency**.

```
```
