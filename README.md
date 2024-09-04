Potato Disease Detection Model
Overview
This repository contains the implementation of a deep learning model for detecting diseases in potato plants. The model leverages Convolutional Neural Networks (CNN) to classify images of potato leaves into healthy or diseased categories. The project includes data preprocessing, model training, evaluation, and deployment using Docker and TensorFlow Serving.

Features
Deep Learning Model: Utilizes CNNs for high-accuracy disease detection.
Data Preprocessing: Includes image augmentation and normalization.
Model Deployment: Dockerized application with TensorFlow Serving for scalable deployment.
Installation
Clone the repository:
git clone https://github.com/yourusername/potato-disease-detection.git
cd potato-disease-detection

Install dependencies:
pip install -r requirements.txt

Data Preprocessing
Image Collection: Gathered a dataset of potato leaf images from various sources.
Annotation: Labeled images as healthy or diseased.
Augmentation: Applied transformations such as rotation, flipping, and scaling to increase dataset size.
Normalization: Scaled pixel values to the range [0, 1].
Model Training
Architecture: Built a CNN model using TensorFlow and Keras.
Training: Trained the model on the preprocessed dataset, using techniques like early stopping and learning rate decay.
Evaluation: Assessed model performance on a validation set, achieving high accuracy.
Deployment
Dockerization: Created a Docker image for the model to ensure consistency across different environments.
TensorFlow Serving: Deployed the model using TensorFlow Serving for real-time predictions.
API Integration: Developed a REST API to interact with the model, allowing users to upload images and receive predictions.
Usage
Run the Docker container:
docker run -p 8501:8501 yourusername/potato-disease-detection

Make predictions:
Use the provided API endpoint to upload images and get disease predictions.
Results
Accuracy: The model achieved a 95% accuracy rate on the test dataset.
Scalability: The deployment setup ensures the model can handle multiple requests simultaneously.
Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

License
This project is licensed under the MIT License.


