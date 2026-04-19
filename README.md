# 🏠 Housing Price Prediction (Machine Learning)

## 📌 Project Overview

This project is a **Machine Learning-based Housing Price Prediction system** built using **Scikit-learn**.
It predicts the **median house value** based on various housing features such as income, location, and population.

---

## 🚀 Features

* Data preprocessing using **Pipeline & ColumnTransformer**
* Handles **missing values and categorical data**
* Model training using **Random Forest Regressor**
* Stratified sampling for better data splitting
* Saves trained model and preprocessing pipeline locally

---

## 🧠 Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Joblib

---

## 📂 Project Structure

```id="projstruct"
project/
│
├── main.py              # Training & inference script
├── housing.csv          # Dataset
├── input.csv            # Generated test input (after running)
├── output.csv           # Predictions (after running)
├── requirements.txt
├── .gitignore
└── README.md
```

---

## ⚙️ How It Works

1. Loads dataset (`housing.csv`)
2. Performs stratified sampling for train/test split
3. Builds preprocessing pipeline:

   * Numerical → Imputation + Scaling
   * Categorical → OneHotEncoding
4. Trains a **Random Forest Regressor**
5. Saves model and pipeline locally (`.pkl` files — not tracked in Git)
6. Performs inference and stores predictions in `output.csv`

---

## 🛠️ Installation & Setup

### 1. Clone the Repository

```bash id="clonecmd"
git clone https://github.com/your-username/housing-price-ml.git
cd housing-price-ml
```

---

### 2. Create Virtual Environment (Optional but Recommended)

```bash id="venvcmd"
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

---

### 3. Install Dependencies

```bash id="reqcmd"
pip install -r requirements.txt
```

---

## ▶️ Running the Project

```bash id="runcmd"
python main.py
```

---

## 📦 Output Files (Generated After Running)

* `model.pkl` → trained model (not included in repo)
* `pipeline.pkl` → preprocessing pipeline (not included in repo)
* `input.csv` → test data
* `output.csv` → predictions

---

## ⚠️ Note

The trained model files (`model.pkl`, `pipeline.pkl`) are **not included in this repository** due to GitHub size limits.

To generate them, simply run:

```bash id="genmodel"
python main.py
```

---

## 📈 Future Improvements

* Add Flask API for deployment
* Dockerize the application
* Deploy on cloud platforms
* Improve model performance

---

## 👨‍💻 Author

Aditya Jhinjha

---

## ⭐ If you found this useful

Give this repo a star ⭐ and feel free to contribute!
