# Algerian Forest Fires - FWI Prediction

A machine learning project that predicts the **Fire Weather Index (FWI)** using weather and fire-related features from the Algerian Forest Fires dataset.

The project covers the complete workflow from data preprocessing and model training to deploying the trained model as a Flask web application.

## Technologies Used

- Python
- NumPy
- Pandas
- Scikit-learn
- Flask
- HTML
- Git & GitHub
- AWS Elastic Beanstalk

## Machine Learning

The project uses **Ridge Regression** to predict FWI.

### Features Used

- Temperature
- Relative Humidity (RH)
- Wind Speed (WS)
- Rain
- FFMC
- DMC
- ISI
- Classes
- Region

Before prediction, the input features are scaled using `StandardScaler`.

The trained model and scaler are saved using Pickle:

```text
models/
├── ridge.pkl
└── scaler.pkl
```
## Project Structure
```text
Algerian Forest Fires Project/
│
├── models/
│   ├── ridge.pkl
│   └── scaler.pkl
│
├── notebooks/
│   ├── Algerian Fires.ipynb
│   ├── Algerian_forest_fires_dataset_UPDATE.csv
│   └── Cleaned_Algerian_forest_fires_dataset.csv
│
├── templates/
│   ├── home.html
│   └── index.html
│
├── .ebextensions/
│   └── python.config
│
├── application.py
├── requirements.txt
├── .gitignore
├── .ebignore
└── README.md
```
## How It Works
```text
Dataset
   ↓
Data Cleaning
   ↓
Exploratory Data Analysis
   ↓
Feature Selection
   ↓
Train-Test Split
   ↓
Feature Scaling
   ↓
Ridge Regression
   ↓
Save Model
   ↓
Flask Web Application
   ↓
FWI Prediction
```

### Run Locally

Clone the repository and install the dependencies:
```bash
pip install -r requirements.txt
```

Run the Flask application:
```bash
python application.py
```

Then open the home page:
```text
http://127.0.0.1:5000/
```

The prediction page is available at:
```text
http://127.0.0.1:5000/predictdata
```

Enter the required weather and fire-related values to get the predicted FWI.


### Deployment

The Flask application is prepared for deployment using AWS Elastic Beanstalk.

## Learning Outcomes

Through this project, I learned and implemented:

- Data preprocessing
- Exploratory Data Analysis
- Feature scaling
- Ridge Regression
- Model serialization
- Flask model deployment
- Git & GitHub
- AWS Elastic Beanstalk deployment


## Author

**Shlok Singh**
