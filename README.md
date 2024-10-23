## Diabetes Prediction Web App

This web application predicts whether a person is diabetic or not based on certain health parameters. It uses a machine learning model trained on the Pima Indians Diabetes Dataset. This project provides a user-friendly interface for early diabetes risk assessment.

https://github.com/user-attachments/assets/5d839800-473e-4302-baab-be470ac56efc

### Aim

The purpose of this project is to help individuals get an early indication of potential diabetes through health parameters and make informed decisions on consulting a healthcare provider.

### Dataset Description

The Pima Indians Diabetes Dataset contains several health-related factors, such as:
- **Pregnancies**: Number of times the person has been pregnant
- **Glucose**: Plasma glucose concentration
- **BloodPressure**: Diastolic blood pressure (mm Hg)
- **SkinThickness**: Triceps skinfold thickness (mm)
- **Insulin**: 2-hour serum insulin (mu U/ml)
- **BMI**: Body Mass Index (weight in kg/(height in m)^2)
- **DiabetesPedigreeFunction**: A function that scores likelihood of diabetes based on family history
- **Age**: Age of the person

### Machine Learning Model

The machine learning model used in this project is **Logistic Regression**, which is a widely-used algorithm for binary classification problems. Here’s how the model was built:
1. **Data Preprocessing**: All data was normalized using `StandardScaler` to ensure that each feature contributes proportionally to the prediction.
2. **Model Selection**: Logistic Regression was selected for its interpretability and efficiency for binary classification.
3. **Integration**: The trained model was integrated with a Flask-based web interface, allowing users to input their health data and get predictions.

### Flask Integration

- **Frontend**: HTML forms are used to collect user inputs (such as glucose levels, BMI, etc.).
- **Backend**: Flask processes the user input, applies the Logistic Regression model, and returns a prediction.

#### How to Use This App

1. Clone the repository:
    ```bash
    git clone https://github.com/tanmay-045/diabetes-prediction-app.git
    cd diabetes-prediction-app
    ```
2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```
3. Run the Flask app:
    ```bash
    python application.py
    ```
4. Visit the app in your browser:
    ```
    http://127.0.0.1:5000/
    ```

### Results

This app helps assess the risk of diabetes based on user-provided health parameters. With an approximate accuracy of 77%, the Logistic Regression model offers reliable predictions and can be used for quick self-assessments.

---

Developed by **Tanmay Sharma**. For more projects, visit my [GitHub](https://github.com/tanmay-045).
