# credit-card-fraud-detection
📌 Project Overview
This project aims to build a machine learning model to detect fraudulent credit card transactions efficiently. The model is trained using a Random Forest Classifier and evaluated based on accuracy, precision, recall, and F1-score. The dataset is imbalanced, so techniques like undersampling/oversampling are used to improve detection.

📊 Dataset Details
Dataset Name: Credit Card Fraud Detection Dataset

Features:

Time: Seconds elapsed since first transaction

Amount: Transaction amount

V1-V28: Anonymized principal components (PCA-transformed features)

Class: Target variable (0 = Not Fraud, 1 = Fraud)

Class Imbalance:

Non-Fraudulent Transactions (0): 99.83%

Fraudulent Transactions (1): 0.17%

🔍 Data Preprocessing Steps
Handling Missing Values: Checked for missing values (None were found).

Feature Engineering:

Extracted TransactionHour from Time.

Applied log transformation to Amount.

Class Balancing: Used SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic fraud samples.

Feature Scaling: Used StandardScaler to normalize data.

Splitting Data: Used an 80-20 split for training and testing.

⚙️ Model Selection & Training
Model Used: Random Forest Classifier

Parameters:

n_estimators = 100

random_state = 42

📈 Model Evaluation Metrics
Metric	Score
Accuracy	XX.XX%
Precision	XX.XX%
Recall	XX.XX%
F1-Score	XX.XX%
📊 Visualizations
✔️ Confusion Matrix to analyze misclassifications
✔️ Feature Importance Graph to understand key features

🚀 How to Run the Project
1️⃣ Install Dependencies
bash
Copy
Edit
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn
2️⃣ Run the Python Script
bash
Copy
Edit
python fraud_detection.py
(Make sure the dataset is in the same directory as the script.)

📜 Conclusion
This project successfully detects fraudulent transactions using a Random Forest model while minimizing false positives. Future improvements can include deep learning techniques like LSTMs or Autoencoders for better fraud detection.

📂 Repository Structure
bash
Copy
Edit
📁 credit-card-fraud-detection  
│── 📄 fraud_detection.py  # Main Python script  
│── 📄 creditcard.csv  # Dataset  
│── 📄 README.md  # Project documentation  
🙌 Acknowledgments
Special thanks to Kaggle for providing the dataset! 🎉
