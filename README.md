# Multi-Target Stance Detection with Adversarial Attention Network (MTAAN)

This repository contains the implementation of MTAAN, a robust stance detection model that combines BERT-based feature extraction with adversarial attention and multi-target handling capabilities. It classifies text stances as *Favor*, *Against*, or *Neutral* towards multiple topics, including unseen ones.

## 🚀 Features
- BERT for contextual word representation
- Adversarial attention mechanism to boost generalization
- Multi-target stance detection
- Discriminator networks for stance and sentiment separation
- Flask backend + Streamlit frontend for deployment

## 📊 Dataset
- **Dataset Name:** SemEval 2016 Stance Dataset
- **Source:** https://www.saifmohammad.com/WebPages/StanceDataset.htm
- **Preprocessing:** Normalization, null handling, train-test split (70:30)

## 📁 Project Structure
```
multi-target-stance-detection/
├── data/                   # Contains datasets and preprocessing scripts
├── models/                 # BERT + Adversarial Attention model files
├── utils/                  # Utility functions
├── app/                    # Flask backend and Streamlit frontend
├── train.py                # Model training script
├── evaluate.py             # Evaluation and metrics script
├── requirements.txt        # Python package requirements
└── README.md               # This file
```

## ⚙️ Setup & Installation

1. Clone this repository
```
git clone https://github.com/YOUR_USERNAME/multi-target-stance-detection.git
cd multi-target-stance-detection
```

2. Create and activate a virtual environment
```
python -m venv venv
source venv/bin/activate    # Linux/Mac
venv\Scripts\activate       # Windows
```

3. Install required packages
```
pip install -r requirements.txt
```

4. Train the model
```
python train.py
```

5. Evaluate model performance
```
python evaluate.py
```

6. Run the web app
```
cd app
streamlit run app.py
```

## 📈 Evaluation Metrics
- Accuracy
- Precision, Recall, F1-Score
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- MAPE (Mean Absolute Percentage Error)
- AUC (Area Under Curve - multi-class)

## 🧠 Technologies Used
- Python
- PyTorch / TensorFlow (based on implementation)
- Transformers (HuggingFace)
- Streamlit
- Flask
- Scikit-learn
- Pandas, NumPy

## 👥 Authors
- G. Greshma
- Lakshmi Priya Yadav
- K. Meghana
- P. Shahina Parveen
- D. Hari Priya

## 📜 License
This project is licensed under the MIT License.
