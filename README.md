# 🔥 ANN-Classification-Customer-Churn

A lightweight **Streamlit app** that predicts whether a customer is likely to churn based on demographic and service-related input features. Powered by a trained TensorFlow model.

![App Screenshot]<img width="1899" height="824" alt="Screenshot 2025-07-18 001526" src="https://github.com/user-attachments/assets/d05e895a-f112-42f0-ac66-32bbee2a40bb" />
<img width="1894" height="826" alt="Screenshot 2025-07-18 001542" src="https://github.com/user-attachments/assets/8423d915-147a-4a9b-8dca-7566904db76d" />

## 🚀 Live Demo

👉 Try the live app on Hugging Face Spaces:  
[https://huggingface.co/spaces/KaustavModak/ann-classification-customer-churn]

---

## 🧠 Model Overview

- Built with **TensorFlow 2.12.0**
- Preprocessing using:
  - `LabelEncoder` (Gender)
  - `OneHotEncoder` (Geography)
  - `StandardScaler` (Numerical features)
- Input features include:
  - Age, Gender, Geography
  - Credit Score, Balance, Tenure
  - Number of Products, Has Credit Card, Is Active Member

---

## 📂 Project Structure

```
.
├── app.py                      # Streamlit frontend
├── model.h5                   # Trained Keras model
├── label_encoder_gender.pkl   # Gender encoder
├── onehot_encoder_geo.pkl     # Geography encoder
├── scaler.pkl                 # Scaler for numerical features
├── requirements.txt           # Python dependencies
├── runtime.txt                # Python version pin
├── README.md                  # This file
```

---

## ⚙️ Setup Instructions

### 🔧 Run locally

```bash
# Clone the repository
git clone https://github.com/yourusername/churn-predictor.git
cd churn-predictor

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run Streamlit app
streamlit run app.py
```


## 📊 Example Prediction

| Feature           | Value      |
|------------------|------------|
| Age              | 35         |
| Gender           | Male       |
| Geography        | France     |
| Credit Score     | 720        |
| Tenure           | 5 years    |
| Balance          | 50000      |
| Products         | 2          |
| Has Credit Card  | Yes        |
| Is Active Member | No         |

✅ **Predicted**: Likely to Stay

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 💡 Credits

Created by [Your Name](https://github.com/KaustavModak)  
Deployed on [Hugging Face Spaces](https://huggingface.co/KaustavModak)
