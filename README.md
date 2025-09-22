# 🌩️ Cloudburst Prediction System  

AI-powered system that uses ERA5 weather data and machine learning to predict cloudburst events.  
Trains a Random Forest model to forecast cloudbursts, evaluate performance, and identify key weather factors for early warning systems.  

---

## 📖 Description  
The **Cloudburst Prediction System** leverages historical ERA5 climate reanalysis data (rainfall, temperature, humidity, wind, etc.) to predict cloudburst events.  
The pipeline includes:  
- Data preprocessing and cleaning  
- Feature engineering  
- Model training using **Random Forest**  
- Performance evaluation (accuracy, precision, recall, F1, ROC-AUC)  
- Feature importance analysis to understand key weather drivers  

This project can serve as a foundation for real-time early warning systems in disaster-prone regions.  

---

## 🚀 How to Run  

### Option 1: Run in Google Colab (Recommended)  
1. Open the notebook in **Google Colab**.  
2. Upload your dataset (`cloudpredictionsystemproject.csv`).  
3. Run each step in order (data loading → preprocessing → training → evaluation → feature importance).  

### Option 2: Run Locally  

1. Clone the repo:  
   ```bash
   git clone https://github.com/yourusername/cloudburst-prediction.git
   cd cloudburst-prediction

2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3. Place your dataset (cloudpredictionsystemproject.csv) in the project folder.

4. Run the pipeline script:
   ```bash
   python cloudburst_model_pipeline.py
5. Outputs will be saved in the model_outputs/ folder:
      - cloudburst_rf_model.pkl → trained model
      - feature_importances.csv → top weather predictors
