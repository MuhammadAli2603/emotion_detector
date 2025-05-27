**Emotion Detection using AI - PyPower Project**

This project demonstrates the use of a Convolutional Neural Network (CNN) for facial emotion detection. Using deep learning, the model classifies facial expressions into different emotion categories.

**Project Overview**

The Emotion Detection system leverages a pretrained model based on the MobileNet architecture and Haar Cascade Classifier for face detection. The goal is to classify facial emotions in real-time from webcam feed or image input.

**Key Features**

Real-Time Emotion Detection: The system detects emotions such as Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral directly from video feed.

Pretrained Models: The system uses a pre-trained model (emotion_model.h5) for classification, trained on facial expression datasets.

Face Detection: A Haar Cascade Classifier is used to detect faces in real-time, providing the region of interest for emotion classification.

Multiple Emotion Categories: The system can identify seven different emotions: Angry, Disgust, Fear, Happy, Sad, Surprise, and Neutral.

**Getting Started**
Follow these steps to get the project up and running:

1. Clone the Repository
bash
Copy
Edit
**git clone :**
 https://github.com/MuhammadAli2603/emotion-detection.git



**File Details**
**1. train.py**
Purpose: Script to train the emotion detection model using the MobileNet architecture.

Libraries Used: Keras, TensorFlow, OpenCV

Model Used: MobileNet with custom fully connected layers on top.

**2. test.py**
Purpose: Script to run emotion detection in real-time using a webcam.

Libraries Used: OpenCV, Keras

Class Labels: The model detects seven emotion categories:

Angry

Disgust

Fear

Happy

Sad

Surprise

Neutral

**3. ali.xml**
Purpose: Pre-trained face detector used to detect faces in real-time before emotion classification.

Note: Ensure that the file path is correctly specified in the script for successful face detection.

**4. emotion_model.h5**
Purpose: Pretrained emotion detection model saved after training.

Structure: A deep CNN model based on MobileNet with a custom top layer for emotion classification.

**Contributions**
Fork the repository, make your changes, and submit a pull request for review.

Feel free to suggest enhancements or file issues if you encounter any bugs.

**Acknowledgements**
Kaggle Dataset: Challenges in Representation Learning - Facial Expression Recognition Challenge

MobileNet Model: MobileNet

OpenCV: OpenCV Documentation
