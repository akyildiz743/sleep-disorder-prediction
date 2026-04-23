Sleep Disorder Prediction: Lifestyle Patterns vs. Clinical Metrics

    This project explores the application of machine learning algorithms to predict sleep disorders (Insomnia and Sleep Apnea). The study uniquely compares two distinct datasets to evaluate how data integrity impacts model performance, ultimately demonstrating the "Garbage In, Garbage Out" (GIGO) principle in health informatics.

📊 Project Overview

    The goal of this research was to determine if daily lifestyle habits (Dataset A) or clinical physiological measurements (Dataset B) serve as better predictors for sleep health.

Key Discovery: The GIGO Principle

    While the lifestyle dataset yielded over 93% accuracy, the clinical dataset—despite containing direct medical metrics like oxygen saturation—resulted in near-random accuracy (~20-30%). A deep dive into the raw data revealed that Dataset B was synthetic and randomly generated, proving that model complexity cannot compensate for flawed data.

🛠️ Technologies & Libraries

    Language: Python
    
    Environment: Jupyter Notebook / VS Code
    
    ML Framework: Scikit-Learn
    
    Data Manipulation: Pandas, NumPy
    
    Visualization: Seaborn, Matplotlib

📂 Datasets

    Dataset A (375 records): Sleep Health and Lifestyle Dataset by Laksika Tharmalingam.
    (https://www.kaggle.com/datasets/851c829b2a41e6dd0b5a60388cd4a2cfda2d54433450ed12141237416c8161bc)
    
    Features: BMI, Blood Pressure, Physical Activity, Stress Level, Occupation.
    
    Dataset B (1,000 records): Sleep Disorder Diagnostic Dataset by ZIYA.
    https://www.kaggle.com/datasets/ziya07/sleep-disorder-diagnostic-dataset
    
    Features: AHI Score, SaO2 (Oxygen Saturation).

🚀 Machine Learning Pipeline

    Feature Engineering: Split compound string variables (Blood Pressure) into numerical Systolic and Diastolic features.
    
    Preprocessing: Applied One-Hot Encoding for categorical data and Standard Scaling for numerical consistency.
    
    Modeling: Implemented and compared three classification algorithms:
    
    Logistic Regression
    
    k-Nearest Neighbors (k-NN)
    
    Random Forest

📈 Results

| Algorithm              | Dataset A (Lifestyle) | Dataset B (Clinical) |
| :--------------------- | :-------------------: | :------------------: |
| **Random Forest** |       **93.33%** |        23.50%        |
| **k-Nearest Neighbors** |         92.00%        |        19.50%        |
| **Logistic Regression** |         90.67%        |        32.00%        |

Random Forest emerged as the superior model for real-world lifestyle data due to its ability to handle non-linear relationships between physical health and sleep quality.

📝 Conclusion

Lifestyle Matters: Simple habits like weight management and blood pressure monitoring are highly effective predictors of sleep disorders.

Data Quality is Critical: The failure of the models on Dataset B highlights that the success of any Pattern Recognition system is entirely dependent on the mathematical integrity of the underlying data.

Author: Abdulkadir Yıldız

Date: April 2026
