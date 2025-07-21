# Weather Prediction
A machine learning project that predicts weather outcomes using historical weather data. This model uses various meteorological features to predict weather conditions with high accuracy.

## Dataset

The model uses a comprehensive weather dataset with the following features:

### Numerical Features
- **MinTemp** - Minimum temperature (°C)
- **MaxTemp** - Maximum temperature (°C) 
- **Rainfall** - Rainfall amount (mm)
- **Evaporation** - Evaporation amount (mm)
- **Sunshine** - Hours of sunshine
- **WindGustSpeed** - Speed of wind gust (km/h)
- **WindSpeed9am** - Wind speed at 9am (km/h)
- **WindSpeed3pm** - Wind speed at 3pm (km/h)
- **Humidity9am** - Humidity at 9am (%)
- **Humidity3pm** - Humidity at 3pm (%)
- **Pressure9am** - Atmospheric pressure at 9am (hPa)
- **Pressure3pm** - Atmospheric pressure at 3pm (hPa)
- **Cloud9am** - Cloud cover at 9am (oktas)
- **Cloud3pm** - Cloud cover at 3pm (oktas)
- **Temp9am** - Temperature at 9am (°C)
- **Temp3pm** - Temperature at 3pm (°C)

### Categorical Features
- **Location** - Weather station location
- **WindGustDir** - Direction of wind gust
- **WindDir9am** - Wind direction at 9am
- **WindDir3pm** - Wind direction at 3pm
- **RainToday** - Whether it rained today (Yes/No)

## 🛠️ Technologies Used

- **Python 3.x**
- **pandas** - Data manipulation and analysis
- **scikit-learn** - Machine learning algorithms and preprocessing
- **NumPy** - Numerical computing
- **Matplotlib/Seaborn** - Data visualization (if applicable)

## 🚀 Model Pipeline

### 1. Data Preprocessing
- **Missing Value Handling**: SimpleImputer for numerical features
- **Feature Scaling**: MinMaxScaler for numerical normalization
- **Categorical Encoding**: OneHotEncoder for categorical variables
- **Train/Validation/Test Split**: Proper data splitting for model evaluation

### 2. Model Training
- **Algorithm**: Random Forest Classifier
- **Features**: Combination of scaled numerical and encoded categorical features
- **Evaluation**: Performance metrics on validation and test sets

### 3. Prediction Function
```python
def predict_input(single_input):
    # Processes single weather observation and returns prediction with probability
    return prediction, probability
```

## 🔧 Installation & Setup

1. **Clone the repository**
```bash
git clone https://github.com/Saanvi-2711/Weather-Prediction.git
cd Weather-Prediction
```

2. **Install required packages**
```bash
pip install pandas scikit-learn numpy matplotlib seaborn
```

3. **Run the notebook**
```bash
jupyter notebook notebooks/RandomForests.ipynb
```

## 🔍 Key Features

- **Robust Preprocessing**: Handles missing values and scales features appropriately
- **Feature Engineering**: One-hot encoding for categorical variables
- **Model Persistence**: Saves trained transformers and model for future use
- **Easy Prediction Interface**: Simple function to make predictions on new data
- **Comprehensive Pipeline**: End-to-end machine learning workflow
