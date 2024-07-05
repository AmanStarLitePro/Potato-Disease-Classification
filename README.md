# Potato Disease Classification
 Detect Early Blight Leaf, Healthy Leaf, Late Blight Leaf 

Welcome to the **Potato Disease Classification** repository! , this project leverages cutting-edge computer vision and machine learning technologies to enhance Potato Leaf Disease Classification.

## 📄 Introduction
This code sets up a FastAPI server that utilizes a pre-trained TensorFlow model to classify images uploaded via API into different classes of potato diseases.
The primary objectives is:
- Detect the Disease in Potato Leaf.

The system integrates CNN Architecture to detect disease in leaf.

## 🗂 Table of Contents
- [Introduction](#-introduction)
- [Requirements](#-requirements)
- [Features](#-features)
- [Data Collection](#-data-collection)
- [API Integration](#-api-integration)
- [Output](#-output)
- [Conclusion](#-conclusion)
- [Get Started](#-get-started)

## 📦 Requirements
1. [Numpy](https://numpy.org/doc/)
2. [uvicorn](https://www.uvicorn.org/)
3. [PIL (Pillow)](https://pillow.readthedocs.io/en/stable/)
4. [Tensorflow](https://www.tensorflow.org/api_docs)
5. [FastAPI](https://fastapi.tiangolo.com/tutorial/)
6. [Postman Software](https://learning.postman.com/docs/introduction/overview/)

## 🎥 Demo Video
![Demo Video](https://github.com/AmanStarLitePro/Potato-Disease-Classification/blob/c5fbc3b6435b31208d9f119d1433bc2bbf15e508)

## 🎯 Features

### 🖼 Object Detection
**Ping Endpoint**
- Responds with "Server is Ready" to indicate the server status.

**Prediction Endpoint**
- Accepts an image file via POST request, processes it using a pre-trained TensorFlow model (my_model.keras), and returns the predicted class and confidence score of the image.

**Output**
- The model outputs predicted class and confidence of prediction.

## Server Access Using Postman Software

- API accessible via the local host server at `http://localhost:8000`.

- Install Postman:

- If you haven't already, download and install Postman from [here](https://www.postman.com/downloads/).
- Create a New Request:

- Open Postman and click on New to create a new HTTP request.
- Set the Request Type and URL:

- Select POST as the request type.
- Enter the API endpoint URL: http://localhost:8000/predict.

- Set Headers:
- Add a new header with key 'Content-Type' and value 'multipart/form-data'. 

- Set the Body:
- Click on the Body tab and Select the "form-data" option.
- Add a new key-value pair where the key is file (must match the parameter name file in your FastAPI endpoint) and the value is the image file you want to classify. You can either drag 
  and drop the image file or select it using the file picker.

- Send the Request:
- Click on Send to submit your request to the API.

- You should receive a response with the predicted class and confidence of prediction.

For more details on using Postman, refer to the [Postman Documentation](https://learning.postman.com/docs/introduction/overview/).

## 📊 Output
![Output](https://github.com/AritriPodde2210/TeleICU-Patient-Monitoring-System/assets/123970201/819a41cb-b4d0-45fe-9d5a-ea6ebfd87f3e)

## 🏁 Conclusion
This project effectively demonstrates the integration of FastAPI with TensorFlow for real-time image classification of potato diseases. By developing endpoints for server status checking and image prediction, utilizing a pre-trained deep learning model, and leveraging tools like Postman for testing, the API proves robust in handling image uploads, processing them with high accuracy, and returning actionable predictions. This solution not only showcases the synergy between modern web frameworks and AI technologies but also highlights its potential impact in agricultural sectors, offering a scalable and efficient tool for disease detection and management, ultimately contributing to improved crop health and productivity.

Future work will focus on improving the models’ accuracy, expanding the dataset, and exploring additional functionalities to enhance the system’s capabilities.

## 🚀 Get Started

**Install Dependencies and Run the API:**

```sh
pip install -r requirements.txt
python main.py

## Access the API:
Open your browser and go to http://127.0.0.1:9000.


Thank you for checking out our project! If you have any questions or feedback, feel free to reach out to us.

