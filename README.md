# Health Insurance Premium Prediction

## Project Overview

This project is an end-to-end machine learning solution designed to predict health insurance premiums for individuals. The primary goal is to build a highly accurate regression model that can estimate insurance costs based on a variety of demographic, health, and lifestyle factors. The project includes data cleaning, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and deployment of a user-friendly web application for real-time predictions.

## Key Features

* **End-to-End ML Pipeline:** Covers the complete machine learning lifecycle from data ingestion to model deployment.
* **Advanced Feature Engineering:** Introduces custom features like `normalized_risk_score` and `genetical_risk` to capture complex relationships in the data and enhance model performance.
* **Demographic Segmentation:** Implements an age-based segmentation strategy, training separate models for "young" (age <= 25) and "rest" (age > 25) populations to improve prediction accuracy for different demographic groups.
* **Comprehensive Model Evaluation:** Utilizes a range of regression algorithms, including Linear Regression, Ridge, Lasso, and XGBoost, with extensive hyperparameter tuning using GridSearchCV and RandomizedSearchCV.
* **High Model Performance:** The final XGBoost model achieves an R-squared score of **94%** on the primary dataset and **88%** on the youth segment, indicating a high degree of accuracy.
* **Interactive Web Application:** A user-friendly interface built with Streamlit allows for easy, real-time premium predictions.
* **Data-Driven Insights:** In-depth EDA provides valuable insights into the factors that most significantly influence insurance premiums.

## How to Run the Project

1.  **Prerequisites:**
    * Python 3.x
    * Git

2.  **Clone the Repository:**
    ```bash
    git clone https://github.com/samim29/ML-Project-Health-Premium-Predict.git
    cd ML-Project-Health-Premium-Predict
    ```

3.  **Install Dependencies:**
    All the required libraries are listed in the `requirements.txt` file. Install them using pip:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Project Structure:**
    ```
    .
    ├── artifacts/
    │   ├── model_rest.joblib
    │   ├── model_young.joblib
    │   ├── scaler_rest.joblib
    │   └── scaler_young.joblib
    ├── .gitignore
    ├── LICENSE
    ├── README.md
    ├── main.py
    ├── prediction_helper.py
    └── requirements.txt
    ```

5.  **Launching the Web Application:**
    To start the interactive prediction application, run the `main.py` file using Streamlit:
    ```bash
    streamlit run main.py
    ```
    This will open a new tab in your web browser with the application interface.
