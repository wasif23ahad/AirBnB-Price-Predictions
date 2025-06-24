# 🏡 Airbnb Price Prediction using ANN

This project is focused on predicting the nightly price of Airbnb listings using structured features from the dataset. It includes comprehensive data cleaning, exploratory data analysis (EDA), feature engineering, and model development using Artificial Neural Networks (ANN) and ensemble techniques.

---

## 📁 Project Structure

📦 Airbnb_Price_Listings/
├── models/
│ └── airbnb_enhanced_ann_model.h5 # Trained ANN model
├── venv/ # Virtual environment (excluded from Git)
├── airbnb_price_listings_predictions.ipynb # Main Jupyter Notebook
├── airbnb.csv # Raw dataset
├── README.md # Project documentation
└── requirements.txt # Python dependencies


---

## 🚀 Features

- ✔️ EDA with visual insights (distribution, correlation, boxplots)
- ✔️ Robust data cleaning (imputation, outlier removal, scaling)
- ✔️ Feature engineering (room density, total rooms)
- ✔️ Model training using ANN with dropout layers
- ✔️ Performance boosting via:
  - Cross-validation
  - GridSearch hyperparameter tuning
  - Ensemble comparisons (Random Forest, Gradient Boosting)
- ✔️ Final model saved in `models/`

---

## 📊 Dataset Overview

The dataset includes the following key fields:
- `rating`, `reviews`, `bedrooms`, `bathrooms`, `guests`, `beds`, `country`
- Text-based fields (amenities, host info) are excluded from modeling for simplicity

Target variable:  
- `price`: Price per night of an Airbnb listing

---

## 🧠 Model Performance

| Model                  | R² Score |
|------------------------|----------|
| Base ANN               | 0.3770   |
| ANN + CV               | 0.3832   |
| Random Forest          | 0.3831   |
| **ANN (Engineered)**   | **↑ Improved** *(final model)*  
| Gradient Boosting      | **↑ Compared** *(if outperforming ANN)*

---

## 🛠️ Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/your-username/airbnb-price-prediction.git
cd airbnb-price-prediction

```

---

2. **Create virtual environment**
```bash
python -m venv venv

# For Windows:
venv\Scripts\activate
# For macOS/Linux:
source venv/bin/activate
```

---

3. **Install packages** 

```bash
pip install -r requirements.txt

```

---

4. **Run the program**

```bash
airbnb_price_listings_predictions.ipynb
```

---

## 📦 Model Export
 ```bash
models/airbnb_enhanced_ann_model.h5

 ```
You can load it with:
```bash
from keras.models import load_model
model = load_model('models/airbnb_enhanced_ann_model.h5')
```

---

## 📌 Author

Mohammad Wasif Ahad
Linkedin: https://www.linkedin.com/in/wasifahad/
Github: https://github.com/wasif23ahad





 
