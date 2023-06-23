![image](https://github.com/keerthikkn/Iris_dataset_classification/assets/42544473/2c5b9a2f-8cd4-45cf-a07c-87d9831941ba)

# Iris Classification Web Application with Flask

This repository contains a simple web application for Iris classification using a Decision Tree Classifier. The Iris dataset is a popular benchmark dataset in the field of machine learning, consisting of measurements of four features (sepal length, sepal width, petal length, and petal width) of three different Iris flower species (Setosa, Versicolor, and Virginica).

The purpose of this web application is to provide a user interface where users can input the measurements of an Iris flower, and the application will classify it into one of the three species using a pre-trained Decision Tree Classifier model.

## Application Features

- User-friendly web interface for entering Iris flower measurements.
- Real-time classification of Iris flowers using the pre-trained model.
- Display of the predicted Iris species on the web page.

## Requirements

The following dependencies are required to run the web application:

- Flask
- scikit-learn
- numpy
- pandas
- requests

These dependencies can be installed by running the command `pip install -r requirements.txt`.

## Usage

To run the Iris classification web application:

1. Install the required dependencies mentioned in the `requirements.txt` file.

2. Ensure that you have the pre-trained Decision Tree Classifier model available. If not, you can train the model using the code provided or load a pre-trained model.

3. Start the web application by running the `server.py` file using the command `python app.py`.

4. Open your web browser and navigate to `http://localhost:5000` to access the application.

5. Enter the measurements of an Iris flower in the input fields and click the "predict" button.

6. The predicted Iris species will be displayed on the web page.

## Docker Image

A Docker image is provided in this repository to facilitate the deployment of the web application.

To create a Docker image and run the web application using Docker, follow these steps:

1. Install Docker on your machine.

2. Build the Docker image using the provided `Dockerfile` by running the following command in the terminal:
   ```
   docker build -t iris-classification-app .
   ```

3. Run the Docker container using the following command:
   ```
   docker run -p 5000:5000 iris-classification-app
   ```

4. Open your web browser and navigate to `http://localhost:5000` to access the application.

## Repository Contents

- `server.py`: Contains the Flask web application code for Iris classification.
- `model.py`: Includes the code for training and saving the Decision Tree Classifier model.
- `Dockerfile`: Specifies the Docker image configuration.
- `requirements.txt`: Lists the required dependencies for running the application.
- `model.pkl` : stores the pretrained model.

## Conclusion

The provided web application demonstrates how to perform Iris classification using a pre-trained Decision Tree Classifier model. Users can input the measurements of an Iris flower through the web interface, and the application will predict its species in real-time.

Please refer to the source code and the accompanying comments for more detailed information about the implementation and customization options for the web application.
