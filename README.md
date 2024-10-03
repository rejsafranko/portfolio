## Professional Projects

### Zdravkec Assistant

I developed Zdravkec Assistant, a comprehensive web application to support medical
professionals. Speech and Vision are two core features. The frontend is developed in Next.js and hosted on
AWS Amplify. The Speech feature integrates OpenAI’s GPT-3.5 to generate structured medical reports
from voice input via Google Cloud Speech transcriptions. This feature enhances the efficiency of report
creation, allowing healthcare providers to document patient information swiftly. The backend is hosted on
AWS EC2, utilizing a CI/CD pipeline with AWS CodePipeline and LifeCycle bash scripts. I also configured
domain management with AWS Route 53 and secured the platform using Nginx with SSL. Payment
processing is handled through Stripe, and user authentication is managed via Google Firebase with a
NoSQL database. Internationalization (i18n) support is also included, ensuring accessibility for a broader
audience. The Vision feature for medical imaging diagnosis runs as a Docker container on Azure Container
Apps. I fine-tuned ResNet50 and MobileNetV2 models in PyTorch on datasets related to brain tumors,
Alzheimer’s, and pneumonia. The application integrates Weights Biases for experiment tracking and model
selection, with the best-performing models uploaded to Azure Blob Storage. GradCAM AI explainability
visualizations highlight critical areas in images that influenced model decisions. To maintain model
performance, Apache Airflow is integrated to monitor for data drifts in the image storage.

### SolarSense

I was responsible for creating a complete solution to detect whether solar panels are dirty. I
built a Typescript API using AWS Lambda and SNS to send real-time notifications from IoT devices. For
the IoT side, I developed a Python script for a Raspberry Pi 3 device which uses MQTT for communication
and a camera for image capturing. Simultaneously, I developed a MobileNetV2 convolutional model to
classify images as clean or dirty. This involved writing scripts to preprocess the data, training models with
TensorFlow, and using Weights and Biases to track experiments and evaluate performance. The device runs
the model locally to classify the captured image of the panels and if needed, triggers SMS/email notification.

### Serverless Suggestion

An MLOps system for a machine learning model which suggests medical services on a health platform. The train and predict methods are deployed as dockerized Python functions on AWS Lambda. The predict Lambda function loads the current model from an AWS S3 bucket, makes a prediction and saves the new input-output pair to the AWS RDS MySQL database. A SQL stored procedure triggers the train Lambda function if there is enough new data entries. Weights&Biases is used for monitoring the training process and selecting which model is uploaded to the AWS S3 bucket.
