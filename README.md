# NASA IMS Bearing Dataset - Predictive Maintenance  

## **Project Overview**  
This project focuses on **Predictive Maintenance (PdM)** using the **NASA IMS Bearing Dataset**. It involves **signal processing, feature extraction, and machine learning models** to detect and predict bearing failures. The dataset contains vibration signals from four bearings running at 2000 RPM under a 6000 lbs radial load.

## **Dataset Description**  
- **Source:** [NASA Prognostics Data Repository](https://ti.arc.nasa.gov/project/prognostic-data-repository)  
- **Data Type:** Vibration signals (ASCII format)  
- **Sampling Rate:** 20 kHz  
- **Test Sets:** 3 test-to-failure experiments  
  - Set 1: Inner race defect (Bearing 3) and roller element defect (Bearing 4)  
  - Set 2: Outer race failure (Bearing 1)  
  - Set 3: Outer race failure (Bearing 3)  

## **Project Workflow**
1. **Exploratory Data Analysis (EDA)**:  
   - Initial investigation and summary statistics  
   - Data visualization using histograms, box plots, and heatmaps  
2. **Feature Engineering & Signal Processing**:  
   - Fast Fourier Transform (FFT) for frequency domain analysis  
   - Wavelet Transform for noise reduction and feature extraction  
   - Statistical features: RMS, Kurtosis, Skewness, Energy, and Entropy  
3. **Machine Learning Models**:  
   - Classical ML models: Logistic Regression, Random Forest, Decision Tree, Naïve Bayes, KNN, SVM, XGBoost  
   - Deep Learning models: CNN, LSTM, CNN-LSTM hybrid  
4. **Remaining Useful Life (RUL) Prediction**:  
   - LSTM and Random Forest for predicting bearing lifespan  
   - Evaluation using Test Loss, MAE, and R² scores  

## **Results Summary**
- **CNN & LSTM models** outperformed classical ML models, achieving **99.6% accuracy**.  
- **Random Forest** showed strong performance for **RUL prediction**.  
- Hybrid **CNN-LSTM** achieved the best balance between feature extraction and time-series forecasting.  

## **Files in This Repository**
- 📄 `Final_Report.pdf` - Detailed report on dataset analysis and model evaluation  
- 📊 `analysis.ipynb` - Jupyter Notebook with data preprocessing, model training, and results  
- 📂 `data.xlsx` - Processed dataset and feature-engineered values  
- 📑 `Literature_review.pdf` - Supporting documentation and findings  
- 📘 `README.md` - This file  

## **Acknowledgments**
This dataset was provided by the **Center for Intelligent Maintenance Systems (IMS), University of Cincinnati**. Special thanks to **NASA Ames Prognostics Data Repository** for making this data publicly available.

---
