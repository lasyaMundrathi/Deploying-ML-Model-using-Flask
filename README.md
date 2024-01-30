# Flower Species Prediction API
This Flask application uses a machine learning model to predict the species of a flower based on the provided sepal length, sepal width, petal length, and petal width. It is a simple and user-friendly web application that receives input through a form and displays the predicted flower species.

## Features
A web form to input flower measurements (sepal length, sepal width, petal length, petal width).
Prediction of the flower species using a pre-trained Random Forest Classifier.
A clean and straightforward UI for easy interaction.
## How to Use
Navigate to the root URL (/). You will see a form with four input fields for the sepal length, sepal width, petal length, and petal width.
Enter the measurements into the form fields.
Click the "Predict" button.
The predicted flower species will be displayed below the form.

#### Input:
![image](https://github.com/lasyaMundrathi/Deploying-ML-Model-using-Flask/assets/98383338/c241c137-d915-4dc3-90b1-f84b0d079b91)

#### Output:
![image](https://github.com/lasyaMundrathi/Deploying-ML-Model-using-Flask/assets/98383338/e65b34f6-ff1c-4ca3-b3d1-3c2c000809b4)

## Installation
To set up the application on your local machine:

Clone the repository to your local machine.
Install the required dependencies by running pip install -r requirements.txt.
Start the Flask server by executing python app.py.
Make sure you have the following Python packages installed:

Flask

Pandas

NumPy

scikit-learn

## Local Development
The app.py file contains the Flask application instance and routes.
The model.pkl file is the serialized Random Forest Classifier model trained on the Iris dataset.
HTML templates are located in the templates folder.
To run the application in development mode, set debug=True in the flask_app.run() call. This enables live reloading and better error reporting.

## Training the Model
The machine learning model was trained on the famous Iris dataset. The following steps were taken:

The dataset was loaded into a Pandas DataFrame.
The data was split into training and testing sets.
Feature scaling was applied to normalize the data.
A Random Forest Classifier was trained on the dataset.
The trained model was serialized into a .pkl file using pickle.
