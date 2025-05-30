

# SolarWiseML

**SolarWiseML** is an integrated machine learning project that combines a user-friendly Flask web app with standalone scripts and a Jupyter notebook to:

* Predict the number of solar panels required based on user input
* Estimate long-term energy savings
* Visualize and explore solar and energy data interactively

---

## 🔹 Key Components

### 1. Web Application (Flask-based)

The Flask app provides a responsive interface that includes:

* Secure login and registration
* Interactive solar panel calculator
* Energy savings estimator
* CSV and PDF download options
* Data visualization (charts and graphs)

> To run:

```bash
cd flask_app
pip install -r requirements.txt
python app.py
```

Then visit `http://localhost:5000` in your browser.

---

### 2. Data Exploration Notebook

Located in `notebooks/data_exploration.ipynb`, this Jupyter notebook is used for:

* Loading and analyzing `solar_data.csv` and `savings_data.csv`
* Preprocessing and feature engineering
* Training regression models (e.g., Linear Regression)
* Exporting models using `joblib` for deployment

---

### 3. Standalone ML Scripts

CLI-based scripts for quick predictions without running the web app:

* `solar_predict.py`: Calculates solar panel requirements
* `savings_predict.py`: Estimates energy savings

Each script prompts for input values and uses a trained `.pkl` model for prediction.

> To run:

```bash
cd ml_scripts
python solar_predict.py  # or savings_predict.py
```

---

### 4. Dataset

CSV files (`solar_data.csv` and `savings_data.csv`) are located in the `data/` directory and used throughout the project for training and testing.

---

## 🔹 Installation

For web app:

```bash
cd flask_app
pip install -r requirements.txt
```

For notebooks and scripts:

```bash
pip install jupyter pandas matplotlib seaborn scikit-learn joblib
```

---

## 🔹 Summary Table

| Module           | Description                                 |
| ---------------- | ------------------------------------------- |
| Flask App        | Interactive UI for prediction and downloads |
| Jupyter Notebook | Data analysis and model training            |
| ML Scripts (CLI) | Terminal-based prediction tools             |
| Data             | Cleaned datasets for model input            |

---

## 🔹 Author

Created by **Yazhini**
Powered by Flask, Scikit-learn, and Linear Regression
