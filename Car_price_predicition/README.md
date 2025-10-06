# Car Price Prediction Model

This project implements a machine learning pipeline to predict car selling prices using various regression models including Random Forest, XGBoost, LightGBM, and CNN.

## Project Overview

The model predicts car selling prices based on features like year, kilometers driven, fuel type, seller type, transmission, owner history, mileage, engine capacity, max power, and number of seats.

## Dataset

The dataset `Cardetails.csv` contains the following features:
- `name`: Car name and model
- `year`: Manufacturing year
- `selling_price`: Target variable (price to predict)
- `km_driven`: Kilometers driven
- `fuel`: Fuel type (Diesel, Petrol, etc.)
- `seller_type`: Type of seller
- `transmission`: Transmission type
- `owner`: Owner history
- `mileage`: Mileage in kmpl
- `engine`: Engine capacity in CC
- `max_power`: Maximum power in bhp
- `torque`: Torque specifications
- `seats`: Number of seats

## Models Implemented

### 1. Random Forest Regressor
- **Performance**: R² Score: 0.9696
- **MAE**: $74,296.09
- **RMSE**: $141,046.63

### 2. XGBoost Regressor
- Extreme Gradient Boosting model for enhanced performance
- Handles non-linear relationships effectively

### 3. LightGBM
- Light Gradient Boosting Machine
- Faster training speed and lower memory usage
- Excellent for large datasets

### 4. CNN (Convolutional Neural Network)
- Deep learning approach for price prediction
- Captures complex patterns in the data

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd car-price-prediction



2.Install required dependencies:
        pip install -r requirements.txt

3.Ensure you have the dataset Cardetails.csv in the project directory.

Usage
        1.Open the Jupyter notebook:
                jupyter notebook Random_Forest_regressor.ipynb
        2.Run all cells to:
                Load and preprocess the data
                Train the Random Forest model
                Evaluate model performance
                Make predictions
        3.For other models (XGBoost, LightGBM, CNN), similar preprocessing and training pipelines are implemented in separate notebooks.

Data Preprocessing:

The preprocessing pipeline includes:

Handling missing values using median imputation for numerical features

One-hot encoding for categorical variables

Standard scaling for numerical features

Feature engineering (extracting numerical values from text fields)


Model Performance:

The current Random Forest model achieves:

R² Score: 0.9696

Mean Absolute Error: $74,296.09

Root Mean Squared Error: $141,046.63

Approximate Average Error: 11.67%

File Structure
car-price-prediction/
├── Random_Forest_regressor.ipynb
├── Cardetails.csv
├── requirements.txt
├── README.md
├── xgboost_model.ipynb
├── lightgbm_model.ipynb
└── cnn_model.ipynb


Key Features

Comprehensive Preprocessing: Handles mixed data types and missing values

Multiple Models: Implements various ML algorithms for comparison

Feature Importance: Analyzes which features most impact car prices

Model Evaluation: Comprehensive metrics for performance assessment


Dependencies

pandas: Data manipulation and analysis

numpy: Numerical computations

scikit-learn: Machine learning algorithms and preprocessing

matplotlib & seaborn: Data visualization

xgboost: Gradient boosting framework

lightgbm: Light gradient boosting machine

tensorflow: Deep learning framework for CNN


Contributing

Fork the repository

Create a feature branch

Commit your changes

Push to the branch

Create a Pull Request


License
This project is licensed under the MIT License.


Contact
For questions or suggestions, please open an issue or contact the maintainers.

You can download these files by:

1. **For requirements.txt**: Copy the content and save as `requirements.txt`
2. **For README.md**: Copy the content and save as `README.md`

To download directly in your environment:

```python
# Save requirements.txt
with open('requirements.txt', 'w') as f:
    f.write('''pandas>=1.5.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.5.0
seaborn>=0.11.0
xgboost>=1.6.0
lightgbm>=3.3.0
tensorflow>=2.8.0
jupyter>=1.0.0
ipykernel>=6.0.0''')

# Save README.md
with open('README.md', 'w') as f:
    f.write('''# Car Price Prediction Model

[Content from above README.md]
''')