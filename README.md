# 🏡 House Price Prediction Using Size, Location, and Neighborhood

A machine learning project that predicts the price of apartments in Buenos Aires using key features such as size, geographic coordinates (latitude and longitude), and neighborhood. Built with Python and scikit-learn, the project applies data preprocessing, feature engineering, pipeline construction, and model training using Ridge regression.

## 📂 Project Structure
├── data/
│ └── buenos-aires-real-estate-*.csv
├── notebook.ipynb
├── requirements.txt
├── Interactive dashboard within notebook
└── README.md


## 🚀 Features

- Cleans and processes real estate listings
- Uses `SimpleImputer`, `OneHotEncoder`, and `Ridge` in a pipeline
- Splits data into training and test sets (80/20)
- Trains a Ridge regression model
- Evaluates model using Mean Absolute Error (MAE)
- Visualizes actual vs predicted values
- Provides an interactive dashboard for predictions using IPyWidgets

## 📊 Dataset

The dataset contains listings for apartments in **Capital Federal, Buenos Aires**. Each entry includes:
- `price_aprox_usd`: target variable (price in USD)
- `surface_covered_in_m2`: apartment size
- `lat`, `lon`: geographic location
- `neighborhood`: area in Buenos Aires

Missing values in `lat` and `lon` are imputed with column means. The `neighborhood` column is one-hot encoded for use in the model.

## 🛠️ Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/Alfred_stack/house-price-prediction.git
   cd house-price-prediction

Create a Virtual Environment to run this Project
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`


📈 Evaluation
Model is evaluated using Mean Absolute Error (MAE). A baseline MAE is calculated using the mean of the target variable, and the trained model's MAE is compared against this baseline to measure improvement.

📉 Visualization
Heatmaps for correlation analysis

Line and scatter plots for predicted vs actual prices

Histograms for data distribution

Interactive sliders for prediction input



💡 Future Improvements
Incorporate more advanced models like XGBoost or Random Forests

Add geospatial visualizations (e.g., Folium map)

Build a full Flask web app for public interaction

📚 References
Scikit-learn documentation: https://scikit-learn.org/

pandas documentation: https://pandas.pydata.org/

Buenos Aires Real Estate Dataset
