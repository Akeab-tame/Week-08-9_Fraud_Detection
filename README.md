# Fraud Detection Project

## Project Overview
This project focuses on building and deploying machine learning models to detect fraudulent activities in e-commerce and bank credit transactions. By using advanced fraud detection techniques, we aim to improve the security of financial transactions and build trust with customers and institutions. Our models will be designed to address challenges like geolocation analysis and transaction pattern recognition for real-time fraud detection.

## Business Need
As a data scientist at Adey Innovations Inc., your task is to create strong fraud detection models to identify fraudulent e-commerce and bank credit transactions. These models will help prevent financial losses, improve transaction security, and streamline real-time fraud monitoring.

### Key Goals:
1. Analyze and preprocess transaction data.
2. Engineer features to highlight fraud patterns.
3. Train and evaluate machine learning models.
4. Deploy models for real-time fraud detection.
5. Create a dashboard to visualize fraud insights.

## Datasets
We will work with the following datasets:

- **Fraud_Data.csv**: E-commerce transaction data for fraud analysis.
  - `user_id`, `signup_time`, `purchase_time`, `purchase_value`, `device_id`, `source`, `browser`, `sex`, `age`, `ip_address`, `class`.
  
- **IpAddress_to_Country.csv**: Maps IP addresses to countries.
  - `lower_bound_ip_address`, `upper_bound_ip_address`, `country`.

- **creditcard.csv**: Bank transaction data for fraud detection.
  - `Time`, `V1-V28` (anonymized features), `Amount`, `Class`.

## Project Structure

### Tasks

1. **Data Analysis and Preprocessing**  
   - Handle missing values.
   - Data cleaning and type correction.
   - Exploratory Data Analysis (EDA).
   - Merge datasets for geolocation analysis.
   - Feature engineering for fraud patterns.
   - Normalize and encode features.

2. **Model Building and Training**
   - Feature and target separation.
   - Train-test split.
   - Train models (Logistic Regression, Random Forest, Gradient Boosting, CNN, LSTM).
   - Model evaluation and improvement.

3. **Model Explainability**
   - Use SHAP and LIME to explain model decisions and improve trust in predictions.

4. **Model Deployment and API Development**
   - Create a Flask API to serve fraud detection models.
   - Dockerize the Flask app for scalable deployment.
   - Implement logging for real-time monitoring.

5. **Dashboard Development**
   - Build a dashboard using Dash to visualize fraud insights (e.g., fraud trends, geographical analysis).

### Prerequisites
- Python 3.8+
- Docker
- Flask
- Dash
- SHAP and LIME libraries
- MLflow for experiment tracking

### Installation
1. Clone the repository:
```bash
   git clone https://github.com/Akeab-tame/Week-08-9_Fraud_Detection
   cd fraud-detection
```
2. Install dependencies:

```bash
pip install -r requirements.txt
```
3. Run the Flask API:

```bash
python serve_model.py
```
4. Build and run the Docker container:

```bash
docker build -t fraud-detection-model .
docker run -p 5000:5000 fraud-detection-model
```
5. Access the dashboard at:

```bash
http://localhost:8050
```
### Features and Technology

- **Modeling:** Logistic Regression, Random Forest, Gradient Boosting, CNN, LSTM.
- **Explainability:** SHAP, LIME for model interpretation.
- **Deployment:** Flask API, Docker.
- **Monitoring:** Logging for fraud detection requests.
- **Dashboard:** Dash for real-time visualization of fraud insights.