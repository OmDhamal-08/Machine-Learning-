
# House Price Prediction Project

## Overview
This project implements a neural network model to predict house prices using the Ames Housing dataset. 
The model processes both numerical and categorical features to make accurate price predictions.

## Features
- Data preprocessing with missing value handling  
- Feature scaling and one-hot encoding  
- Neural network implementation using TensorFlow/Keras  
- Comprehensive model evaluation metrics  
- Visualization of training progress and results  

## Installation

### Prerequisites
- Python 3.7+  
- pip package manager  

```bash
# Clone this repository
git clone <repository-url>
cd house-price-prediction

# Install required dependencies
pip install -r requirements.txt
```

## Usage

### 1. Data Preparation
- Place the `train.csv` file in the project directory  
- The notebook will automatically handle data loading and preprocessing  

### 2. Running the Model
```bash
jupyter notebook house_predictions.ipynb
```
- Execute all cells in sequence  
- The model will train for 40 epochs  

### 3. Interpreting Results
- Model performance metrics are displayed after training  
- Visualization of training progress and predictions are generated  

## Dataset
- The project uses the Ames Housing dataset containing:  
  - 79 explanatory variables  
  - Both numerical and categorical features  
  - House sale prices as the target variable  

## Project Structure
```
house-price-prediction/
├── house_predictions.ipynb   # Main Jupyter notebook
├── requirements.txt          # Python dependencies
├── README.md                 # Project documentation
└── train.csv                 # Dataset file
```

## Model Architecture
- The neural network consists of:  
  - Input layer matching processed feature dimensions  
  - 3 hidden layers with 128, 64, and 32 neurons (ReLU activation)  
  - Output layer with 1 neuron for regression  

## Results
- The model achieves:  
  - Test MAE: ~$19,093  
  - Average error: ~10.68%  
  - Sample prediction: $142,628.94 vs actual: $154,500.00  

## Files
- `house_predictions.ipynb` - Main Jupyter notebook with complete implementation  
- `requirements.txt` - Python dependencies  
- `README.md` - This documentation file  

## License
This project is licensed under the MIT License - see the LICENSE file for details.  

## Acknowledgments
- Dataset source: Ames Housing dataset  
- Built with TensorFlow, scikit-learn, and pandas  


## Screenshots of the Curves
  <img width="1610" height="537" alt="Screenshot 2025-09-18 213104" src="https://github.com/user-attachments/assets/5b61f867-06ee-46a5-9bad-feef3e22b5c3" />
