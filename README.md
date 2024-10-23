# Predictive Modeling for Medication Adherence

![Predictive Modeling for Medication Adherence](https://github.com/user-attachments/assets/afd65627-17bd-464c-bdd6-08edeb45509d)


This project focuses on developing machine learning models to predict medication adherence, specifically targeting patients with HTN, DBT, and STN conditions. The models leverage various demographic and socioeconomic factors to identify patients at risk of poor medication adherence. The primary goal is to enhance healthcare outcomes by predicting non-adherence and enabling timely interventions.

## Project Overview

The project uses **Random Forest** and **XGBoost** to predict medication adherence. It incorporates features such as "total gaps" and "high copay," which were engineered to improve prediction accuracy. Both continuous and categorical variables are handled effectively using Python libraries, and the model's performance is tracked using **MLflow**.

### Key Features

- **Predictive Models**: Random Forest and XGBoost models built to predict patient adherence to medications.
- **Feature Engineering**: Added features like total gaps and high copay to enhance model accuracy.
- **High Accuracy**: Achieved ROC-AUC scores of 0.99 (Random Forest) and 0.98 (XGBoost).
- **Model Tracking**: Models and metrics are logged and tracked using MLflow.

## Technologies Used

- **Python**: For data preprocessing, feature engineering, and model development.
- **Scikit-learn**: For building Random Forest and XGBoost models.
- **Pandas**: For data manipulation and feature extraction.
- **MLflow**: To track model performance and logs.
- **Rest API**: For serving the model.
- **AWS**: For deploying the model and handling infrastructure.

## Getting Started

### Prerequisites

- Python 3.x
- Required libraries (install via `requirements.txt`):
  ```bash
  pip install -r requirements.txt
  ```

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/medication-adherence-predictor.git
   ```
2. Navigate to the project directory:
   ```bash
   cd medication-adherence-predictor
   ```

3. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Prepare the dataset and ensure it is placed in the appropriate directory (`/data` folder).
2. Run the model training:
   ```bash
   python train_model.py
   ```

3. To serve the model via a REST API:
   ```bash
   flask run
   ```

## Results

- The model achieved a **ROC-AUC score of 0.99** (Random Forest) and **0.98** (XGBoost).
- Insights gained from this model help in identifying high-risk patients for early intervention.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
