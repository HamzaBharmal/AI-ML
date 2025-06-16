
# 🏠 Real Estate Price Prediction

This project focuses on predicting real estate prices using a dataset containing property features like transaction date, house age, proximity to public transport, and more. The notebook includes data preprocessing, exploratory data analysis (EDA), model training using regression algorithms, and evaluation.

## 📁 Project Structure

```
.
├── code.ipynb         # Main Jupyter Notebook with all code
├── Real_Estate.csv    # Dataset used for training and analysis
└── README.md          # Project overview and instructions (you are here)
```

## 📊 Dataset Overview

The dataset `Real_Estate.csv` includes the following columns:

| Column Name                    | Description                                      |
|-------------------------------|--------------------------------------------------|
| `No`                          | Row number (serial index)                        |
| `X1 transaction date`         | Date of transaction (decimal format)             |
| `X2 house age`                | Age of the house in years                        |
| `X3 distance to MRT station`  | Distance to nearest public transportation (MRT)  |
| `X4 number of convenience stores` | Number of stores nearby                    |
| `X5 latitude`                 | Latitude coordinate of the house                 |
| `X6 longitude`                | Longitude coordinate of the house                |
| `Y house price of unit area`  | Target column - house price per unit area        |

## 📌 Key Features of the Project

- ✅ Data loading and cleaning using `pandas`
- 📈 Exploratory Data Analysis (EDA) with `matplotlib` and `seaborn`
- 🔍 Correlation analysis between features
- 🧠 Machine Learning model building using:
  - Linear Regression
  - Decision Tree Regressor
  - Random Forest Regressor
- 📊 Model evaluation using:
  - Mean Absolute Error (MAE)
  - Mean Squared Error (MSE)
  - R² Score
- 📉 Prediction visualization and residual analysis

## 🛠️ Requirements

To run this project, ensure you have Python and the following libraries installed:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## 🚀 How to Run the Code

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/real-estate-price-prediction.git
   cd real-estate-price-prediction
   ```

2. Open the Jupyter Notebook:
   ```bash
   jupyter notebook code.ipynb
   ```

3. Run the notebook cells one by one to:
   - Load and explore the data
   - Visualize the relationships
   - Train ML models
   - Evaluate performance

## 📌 Results

- Random Forest performed best with the highest R² score.
- The correlation heatmap showed that `distance to MRT` has a strong negative correlation with price.
- Features like age and number of stores also have noticeable influence.

## 📈 Future Improvements

- Hyperparameter tuning using GridSearchCV
- Add more models (e.g., XGBoost, SVR)
- Deploy as a web app using Streamlit or Flask
- Incorporate additional features like crime rates or school rankings

## 👨‍💻 Author

**Hamza Bharmal**  
Pursuing B.Sc. in Data Science  
[LinkedIn](https://www.linkedin.com/in/hamza-bharmal) | [GitHub](https://github.com/HamzaBharmal)

---

