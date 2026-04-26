# 🌾CROP YIELD PREDICTION

Predicting crop yield using environmental and agricultural factors crucial for informed agricultural decisions. 
It implements an end-to-end deep learning pipeline including preprocessing, feature scaling, model training, and evaluation using TensorFlow (Keras). The project highlights how AI can support data-driven decision-making in agriculture.

## 🎯 Problem Statement
Accurate crop yield prediction helps farmers, policymakers, and agricultural planners optimize resources, reduce losses, and improve food security. This project explores how deep learning can model complex, non-linear relationships between environmental and farm-related features to estimate crop yield.

## 📊 Dataset

The dataset contains agricultural data with both categorical and numerical features:
*  Categorical:
   *   Region
   *   Soil_Type
   *   Season
*   Numerical:
    *   Rainfall
    *   Temperature
    *   Fertilizer
    *   Irrigation
    *   Area

## Target

*  Crop_Yield_ton_per_hectare 

📁 Dataset used in notebook:
```
Crop-yield Dataset.csv
```

## 🔧 Technologies Used

*   Python
*   Jupyter Notebook
*   Pandas, NumPy
*   Matplotlib, Seaborn
*   Scikit-learn
*   TensorFlow / Keras

## 🧪 Model Workflow
1.   Data Preprocessing
*   Label Encoding for categorical features (Region, Soil_Type, Season)
*   Feature scaling using:
    *   StandardScaler
    *   MinMaxScaler
*   Train / Validation / Test split

2.   Models Used
Two Deep Learning models were trained:
*   Model 1
    *   Fully Connected Neural Network
    *   Dense layers with relu and gelu activations
    *   Baseline deep learning model
*   Model 2 
    *   Improved neural network architecture
    *   Better feature scaling and generalization
    *   Reduced prediction error compared to Model 1

3.   Evaluation Metric
*   Mean Absolute Error (MAE)

Predicted values were inverse-transformed to obtain actual crop yield values in tons per hectare

## 📈 Results

*   Mean Absolute Error (MAE): ~0.013 tons/hectare
*   The model captures non-linear relationships in agricultural data effectively
*   Strong generalization observed on unseen test data

The results demonstrate the effectiveness of deep learning models for crop yield prediction.

## 📁 Project Structure
```
Crop_Yield_Prediction/
├── data/
│ ├── Crop-yield Dataset.csv
├── notebook/
│ ├── Crop_yield.ipynb
├── requirements.txt
└── README.md
```

## 🚀 How to Run

1.   Clone the repository
```
git clone https://github.com/your-username/crop-yield-prediction.git
cd crop-yield-prediction
```

2.   Install dependencies
```
pip install -r requirements.txt
```

3.   Run the notebook
```
jupyter notebook notebook/Crop_yield.ipynb
```

## 🔮 Future Improvements
*   Hyperparameter tuning for neural networks
*   Comparison with traditional machine learning models
*   Integration of real-time weather data
*   Deployment as a web application using Streamlit

## 📌 Key Takeaways
*   Hands-on experience with deep learning for regression tasks
*   Real-world application of AI in agriculture 🌱
*   Understanding the impact of preprocessing and scaling on model performance
