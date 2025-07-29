##Face Recognition Pipeline:
This project implements a real-time face recognition pipeline using OpenCV and deep learning techniques in Python. It captures face images from a live video stream, preprocesses the data, trains a model (using Keras), and performs face recognition on incoming video frames.

##Key Features:
Data Collection: Automatically captures 100 face images per person from a webcam or IP camera using Haar Cascade detection.

Data Preprocessing: Converts collected images to grayscale, resizes them, labels them, and serializes the dataset for training.

Face Recognition: Loads a trained deep learning model to recognize faces in real-time from a live video source.

Easy to Use: Modular Python scripts for each stage — collection, preprocessing, and recognition.

##Project Structure:
collect_data.py – Captures faces and saves images.

consolidated_data.py – Prepares and pickles dataset.

recognize.py – Real-time face recognition script.

haarcascade_frontalface_default.xml – Haar Cascade for face detection.

images/ – Raw face images dataset (auto-generated).

clean data/ – Processed dataset storage.

##Usage:
Run collect_data.py to capture images for each face.

Use consolidated_data.py to preprocess images and prepare data for training.

Train your model (not included here) or use an existing .h5 Keras model.

Execute recognize.py for live face recognition.

##Requirements:
Python 3.x

OpenCV

Keras with TensorFlow backend

NumPy

##Notes:
Replace any hardcoded paths in the scripts with your relative project paths.

Ensure your webcam or IP camera URL is configured properly.

The project can be extended with additional models, dataset improvements, and UI enhancements.
