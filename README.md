# Live-Emoji-Detection-
Live emoji detection uses a neural network to recognize facial expressions in real-time and display corresponding emojis. It involves capturing facial landmarks with MediaPipe and OpenCV, training a model on this data, and using the model to predict and show emojis based on live video feed.

The data_training.ipynb file appears to contain a neural network training script for classifying different categories, possibly related to emotions or facial expressions. Here is a brief description of its contents:

The data_training.ipynb file appears to contain a neural network training script for classifying different categories, possibly related to emotions or facial expressions. Here is a brief description of its contents:

Libraries and Initialization: The script imports necessary libraries, including numpy, os, cv2, and tensorflow.keras.

Data Loading and Preprocessing: It loads .npy files containing data and labels, preprocesses the data, and converts labels to categorical format.

Model Definition: A neural network model is defined using Keras, consisting of an input layer, two dense layers with ReLU activation, and an output layer with softmax activation.

Training: The model is compiled with categorical cross-entropy loss and RMSprop optimizer, and trained for 50 epochs.

Saving: The trained model and labels are saved to files.


The face_recog.ipynb file appears to focus on capturing and processing facial landmarks using MediaPipe. Here is a brief description of its contents:

Libraries and Initialization: The script imports necessary libraries, including mediapipe, numpy, and cv2.

Video Capture and Data Collection: It uses OpenCV to capture video from the webcam and prompts the user to enter a name for the dataset.

Facial and Hand Landmark Detection: Using MediaPipe's holistic model, it detects and processes facial and hand landmarks, normalizing the coordinates.

Data Saving: The collected landmark data is saved to a .npy file.



The inference.ipynb file appears to be focused on running inference using a pre-trained model for emotion or expression detection. Here is a brief description of its contents:

Libraries and Initialization: The script imports necessary libraries, including mediapipe, numpy, and cv2.

Model Loading: It loads a pre-trained model and the corresponding labels.

Video Capture and Real-time Inference: It uses OpenCV to capture video from the webcam and MediaPipe to detect facial and hand landmarks.

Prediction and Display: The captured landmarks are passed to the model to predict the expression, which is then displayed on the video feed.
