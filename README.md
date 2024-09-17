# Machine_learning  
## Overveiw  
This project is designed to help students choose the most suitable career path based on their skills, academic performance, and interests. By using a machine learning model, the system provides personalized career recommendations to guide students in making informed decisions about their future.  
  
## **Data**
The dataset used for this project can be found [HERE](https://github.com/loobiish/Student-Career-Prediction).  
It contains various attributes related to student preferences and interests, which are used to train the machine learning model.  
  
## **Libraries**
To run this project, you need to install the required dependencies listed in the requirements.txt file. You can install them using:  
```python
pip install -r requirements.txt 
```  
## **Model Development**  
We built and trained a classification model to predict career recommendations based on student input. Below are the steps involved in model creation:  
### **1. Data Preprocessing**  
* **Missing Data:** Checked for any missing values and handled them appropriately.
* **Duplicate Entries:** Removed any duplicate records in the dataset to avoid bias in the model.
* **Feature Engineering:** Combined similar features to create more meaningful and fewer features, simplifying the model without losing critical information.
  
### **2. Model Selection**  
We tested multiple machine learning models and selected Random Forest for its performance. This model provided the highest accuracy and recall, making it the best fit for this classification task.  
  
## **Evaluation Metrics**  
We evaluated the model using several metrics to ensure its performance. Here are the results:

* Accuracy: 92.11%
* Precision: 93.04%
* Recall: 95.65%
* F1 Score: 93.79%
These metrics indicate that the model performs well in recommending careers based on the input data.

## **Future Work**
Here are a few potential improvements and future plans for the project:

* **Enhance Model Features:** Collect more student-related data to include additional features like extracurricular activities and internships.
* **Explore More Models:** Experiment with other classification algorithms like SVM to potentially improve accuracy.
* **User Feedback:** Incorporate a feedback system where users can provide input on the recommendations, helping the model improve over time.
  
## **Sources**
The dataset and inspiration for this project are taken from [this GitHub repository](https://github.com/loobiish/Student-Career-Prediction).  
  
# **Step-by-Step Guide to Run the Flask Application Locally**  
  
## **1- Install Python:**  
* Ensure you have Python installed on your system. You can download it from the [official Python website](https://www.python.org/downloads/).  
  
## **2- Install the Required Libraries:**  
* install all the dependencies by running:
```python
pip install -r requirements.txt 
```  
  
## **3- Run model.py**
```python
python model.py
```  
## **4- Save Your Model:**  
* Ensure the career_prediction_model.joblib file (your trained model) is saved in the same directory as the app.py file.
  
## **5- Run the Application:**  
* Navigate to the folder where app.py is located and run the Flask application using:
```python
  python app.py
```
  
## **6- Access the Application:** 
* After running the command, Flask will start a local web server. Open your web browser and go to:
```
http://127.0.0.1:5000/
```
* You'll see the form where you can enter your preferences (drawing, sport, coding, etc.) and submit the form to receive a career recommendation.

## **7- Shutting Down:**
* To stop the application, go back to your terminal and press **Ctrl + C.**
