# Career Prediction API

## Overview
This API helps in predicting a student's potential career path based on their educational background, skills, and other relevant characteristics. The prediction model is trained on data from Kaggle, and the API offers endpoints for tasks like data preprocessing, training the model, generating predictions, and evaluating the model's performance.

## Base URL
All API requests are made to this base URL:  
http://127.0.0.1:5000/

## Prerequisites
To use the API, make sure you have the following:
- Python installed.
- Necessary libraries:
  - Pandas, NumPy, Matplotlib, Seaborn
  - scikit-learn (specifically the RandomForestClassifier)
  - joblib for saving/loading models
  - Data visualization libraries like Matplotlib or Seaborn

## How to Use the API

### 1. Start the Flask App:
Ensure the Flask application is running. Start it by running python app.py (or replace app.py with the name of your script).

### 2. Access the Home Page:
Open a web browser and go to http://127.0.0.1:5000/. Here, you'll see a form where users can input their preferences for different activities.

### 3. Submit Preferences:
Fill out the form with 1 for yes or 0 for no for questions like:
- Do you like drawing?
- Do you enjoy sports?
- Do you like coding?
- Are you interested in physics, economics, geography, or science?

### 4. View Recommendations:
After submitting the form, the API will display a career recommendation based on the input provided.

## API Output
The response page will include:
- A heading like "Your Career Recommendation"
- A paragraph detailing the recommended career
- The recommended career itself displayed prominently
- A link to return to the form for more inputs

## How It Works
1. Form Submission: Users input their preferences into a form.
2. Model Loading: The career_prediction_model.joblib is loaded.
3. Prediction: The machine learning model predicts the user’s career path based on the provided inputs.
4. Results Display: The prediction is shown on an HTML page as a career recommendation.

## Additional Information

- Data Source: The dataset used for model training is available at: GitHub Career Prediction Dataset
- Algorithm: The model uses a RandomForestClassifier, an ensemble method that builds multiple decision trees and returns the mode of the predicted classes.
