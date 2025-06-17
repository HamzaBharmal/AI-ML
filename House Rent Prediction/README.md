# 🏡 House Rent Prediction using Machine Learning

This project demonstrates a machine learning pipeline for predicting house rent prices using a dataset of real estate listings. It includes data preprocessing, visualization, feature engineering, and training a predictive model using regression techniques.

---

## 📁 Project Structure

```
.
├── code.ipynb              # Jupyter notebook with complete code
├── House_Rent_Dataset.csv  # Dataset used for training and evaluation
└── README.md               # Documentation file
└── requirements.txt        # Dependencies
```

---

## 🚀 Getting Started

### ✅ Prerequisites

Install the required packages (using pip):

```bash
pip install pandas matplotlib seaborn scikit-learn
```

Alternatively, create a virtual environment:

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

---

## 📊 Dataset Overview

**Filename**: `House_Rent_Dataset.csv`  
**Rows**: ~4700  
**Columns**:
- `BHK`: Number of bedrooms
- `Size`: Size in square feet
- `Area Type`: Super Area / Carpet Area
- `City`: City where the house is located
- `Furnishing Status`: Furnished / Semi-Furnished / Unfurnished
- `Tenant Preferred`: Type of preferred tenant
- `Bathroom`: Number of bathrooms
- `Point of Contact`: Contact method
- `Rent`: Target variable (monthly rent)

---

## 🧠 What the Code Does

1. **Data Loading & Exploration**
   - Loads the dataset using `pandas`
   - Performs initial EDA (null value check, shape, datatype inspection)

2. **Visualization**
   - Uses `matplotlib` and `seaborn` to generate:
     - Correlation heatmaps
     - Distribution plots
     - Box plots for outliers
     - Rent trends per city, furnishing status, BHK, etc.

3. **Data Cleaning**
   - Drops unnecessary columns (e.g., `Point of Contact`)
   - Encodes categorical variables using `LabelEncoder`
   - Handles outliers and checks skewness

4. **Model Building**
   - Splits the data into training and test sets
   - Trains using a **Linear Regression** model from `sklearn`
   - Evaluates using:
     - R² Score
     - Mean Absolute Error (MAE)
     - Mean Squared Error (MSE)
     - Root Mean Squared Error (RMSE)

5. **Prediction**
   - Predicts rent on test data
   - Compares actual vs predicted rent in a DataFrame

---

## 🧪 How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/house-rent-prediction.git
cd house-rent-prediction
```

2. Launch the Jupyter Notebook:

```bash
jupyter notebook code.ipynb
```

3. Run the cells sequentially to understand each stage of the pipeline.

---

## 📈 Sample Output

Model Evaluation Metrics (example):
- R² Score: `0.58`
- MAE: `4500`
- RMSE: `7000`

> Note: Performance may vary based on dataset quality and feature engineering.

---

## 📌 Future Improvements

- Use advanced models (Random Forest, XGBoost, etc.)
- Deploy model using Flask or Streamlit
- Add hyperparameter tuning using GridSearchCV
- Improve feature selection and scaling

---

## 🤝 Contributing

Pull requests and suggestions are welcome! Open an issue to discuss potential changes.

---

