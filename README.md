## Professional Projects

### Speech To Text Medical Assistant

A web application built with Next.js, Node.js and AWS for helping medical professionals create reports by voice input. It uses OpenAI’s GPT 3.5 to generate a structured medical report from a voice transcription generated by Google CloudSpeech. The app is deployed on AWS Amplify and EC2 and integrates Stripe payment, Google Firebase authentication, a Firebase NoSQL database and i18n language switching.

### ImageAid

A web application built in Next.js and Flask for assisting medical imaging diagnosis. It is deployed as a dockerized Flask server on Azure Container Apps. The API serves predictions and GradCAM visualizations from ResNet50 and MobileNetV2 PyTorch models fine-tuned on medical datasets representing brain tumors, Alzheimer’s
disease and pneumonia cases. Model development process uses Weights&Biases for experiment tracking and uploading the best model to Azure Blob Storage. The backend uses a factory method pattern for model object creation to keep the API intact while integrating new models for new diseases. Apache Airflow runs periodical checks of the image storage to detect data drifts.

### Serverless Suggestion

An MLOps system for a machine learning model which suggests medical services on a health platform. The train and predict methods are deployed as dockerized Python functions on AWS Lambda. The predict Lambda function loads the current model from an AWS S3 bucket, makes a prediction and saves the new input-output pair to the AWS RDS MySQL database. A SQL stored procedure triggers the train Lambda function if there is enough new data entries. Weights&Biases is used for monitoring the training process and selecting which model is uploaded to the AWS S3 bucket.

## Academic Projects

### Movie Recommendation Sytem

A machine learning engineering project which aims to create a movie recommendation model based on custom collaborative filtering. We've created an MLOps system for model deployment with a Flask server, Apache Airflow orchestration for model retraining, MLflow model management, PostgreSQL database and MinIO model storage.

### Fish Cultivation Classifier

An academic effort in computer vision engineering which focuses on development of a fish cultivation classifier. The dataset is owned by the Institute of Oceanography and Fisheries of Croatia. I display the use of data augmentation, a Huggingface Vision Transformer (ViT), and a Tensorflow ResNet50 architecture for achieving accurate and robust classification results. Additionally, I've implemented a Grad-CAM visualizer for AI explainability, providing insights into the model's decision-making process.

### Song Lyric Generation with Deep Models

A natural language processing research project which aims to create song lyric generators using various deep learning models with PyTorch and Tensorflow. We have implemented four generators in total. Two for generic lyric generation and two for specific artist lyric generation. The models were trained on a song lyric datset created from 2 different data sources and evaluated through human assessments to ensure the generated lyrics are meaningful and stylistically accurate.

## Personal Projects

### NBA Shot Predictor

A machine learning engineering project which aims to build a classification model for predicting wheter a shot attempt was a score or a miss. I have created an MLOps system for model deployment which consists of a Flask server, a PostgreSQL database and an Apache Airflow workflow orchestration for model retraining.
