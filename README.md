# 🌍 Air Quality Classification using ANN

This project uses an Artificial Neural Network (ANN) to classify air quality as **Hazardous** or **Safe**, based on environmental features like PM2.5, Temperature, Humidity, and various pollutants. It includes data preprocessing, model training, evaluation, and visualization.

## 📁 Dataset

- **Name**: `global_air_quality_data_10000.csv`
- **Format**: CSV
- **Features Used**:
  - `PM2.5`
  - `Temperature`
  - `Humidity`
  - `PM10`
  - `CO`
  - `NO2`
  - `SO2`

The label is created based on PM2.5 values:
- `Hazardous (1)` if PM2.5 ≥ 60
- `Safe (0)` if PM2.5 < 60

## 🔧 Project Workflow

1. **Import Libraries**
2. **Load and Clean Dataset**
3. **Create Binary Labels**
4. **Select Relevant Features**
5. **Balance the Dataset** using upsampling
6. **Feature Scaling** with `StandardScaler`
7. **Train-Test Split**
8. **Build and Compile ANN Model**
9. **Train with Callbacks**: `EarlyStopping` & `ReduceLROnPlateau`
10. **Evaluate Model** using Accuracy, Classification Report, and Confusion Matrix
11. **Visualize** training metrics

## 📊 Model Architecture

- Input Layer: 128 neurons, ReLU
- Hidden Layer 1: 64 neurons, ReLU
- Hidden Layer 2: 32 neurons, ReLU
- Output Layer: 1 neuron, Sigmoid
- Dropout: Used to reduce overfitting (rates: 0.3 and 0.2)

## ✅ Performance Metrics

- **Accuracy**
- **Classification Report**
- **Confusion Matrix**
- **Training & Validation Curves**

## 📈 Visualizations

- Confusion Matrix (heatmap)
- Accuracy vs Epochs
- Loss vs Epochs

## 💡 Requirements

Install dependencies using pip:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow
