** Disease Prediction using Machine Learning**

A machine learning project that analyzes and predicts lung, skin, and kidney diseases using Exploratory Data Analytics (EDA) and classification models.

Built as part of the UCSC318L: Exploratory Data Analytics course at VIT Vellore (WINSEM 2025–2026).


 Team Members

NameReg :
Yamini M 24BCS0034
Naveen Kumar K 24BCS0003
Uvathika U 24BCS0056


Problem Statement

Health conditions like lung disease, skin disorders, and kidney diseases are rising due to environmental pollution, unhealthy lifestyles, and genetic factors. Early detection is critical.

This project performs EDA on merged medical datasets to uncover patterns and risk factors, then builds predictive ML models to classify disease occurrence.


 Dataset

Two datasets were merged using patient_id:

Dataset 1 — Lung Disease


Age, Gender, Smoking Habit, BMI, Lung Score, Disease Status


Dataset 2 — Kidney & Skin Disease


Blood Pressure, Sugar Level, Cholesterol, Alcohol Consumption, Skin Condition


Total Records: 500+ patients

Target Variable: is_disease (0 = Healthy, 1 = Disease)


 Data Transformation Steps


Data Cleaning — Median imputation for missing values
Dataset Merging — Joined on patient_id
Label Encoding — Encoded categorical features (Gender, Smoking, Alcohol, Skin Condition)
Feature Scaling — Applied StandardScaler for normalization
Feature Selection — Removed non-contributing attributes



 EDA Visualizations

PlotPurposeHistogramAge, BMI, Blood Pressure distributionBar ChartSmoking vs DiseaseCount PlotDisease class distributionBox PlotSugar Level vs DiseaseScatter PlotSugar Level vs Disease occurrenceCorrelation HeatmapRelationships between all featuresPie ChartSkin Condition vs DiseaseLine ChartAge distribution trend

Key Insights:


Smoking increases risk of lung disease
High sugar levels are linked to kidney disease
High BMI is associated with greater health risk
Age plays an important role in disease occurrence



 Machine Learning Models

Three classifiers were trained and evaluated:

ModelAccuracyPrecisionRecallF1-ScoreLogistic Regression67%0.4490.670.538Decision Tree58%0.5600.580.568Random Forest65%0.5590.650.558

Best Model: Logistic Regression (67% accuracy)

Most Reliable: Random Forest (handles complex feature relationships best)


 Tech Stack


Language: Python
Libraries: Pandas, Scikit-learn, Matplotlib, Seaborn
Tools: Jupyter Notebook



 How to Run

bash# Clone the repository
git clone https://github.com/yaminimoorthy13-dot/disease-prediction-ml.git
cd disease-prediction-ml

# Install dependencies
pip install pandas scikit-learn matplotlib seaborn

# Run the notebook
jupyter notebook disease_prediction.ipynb


 Project Structure

disease-prediction-ml/
│
├── datasets/
│   ├── lung_disease.csv
│   └── kidney_skin_disease.csv
│
├── disease_prediction.ipynb   # Main notebook
├── README.md


Future Work


Use real-world clinical datasets for better accuracy
Explore deep learning models (Neural Networks)
Deploy as a web app for healthcare professionals
Add more disease categories



License

This project was submitted as an academic course project at VIT Vellore. For educational use only.
