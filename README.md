# Drowsiness Detection System with Emotion Analysis

This project aims to develop a facial recognition system that can be implemented in motor vehicles to enhance security and improve the driving experience. The system utilizes facial expressions to predict if the driver is drowsy or under the influence, providing an alert to prompt them to take a break or avoid further driving. Additionally, an emotion detection system is incorporated to analyze the user's facial expressions and create a personalized in-cabin experience based on their mood, which could involve customized lighting, music, or a combination of both. The system also integrates voice analysis to identify if the user is distressed beyond their natural levels, enabling alerts to be sent to their physicians or family members.

# Importance

Drowsy drivers pose a significant risk on the roads and are a major cause of car accidents, leading to loss of life and property damage. In the United States alone, it is estimated that around 150 deaths per year can be attributed to tired drivers, resulting in 71,000 injuries and $12.5 billion in losses [1]. The financial burden of drowsiness-related accidents amounts to approximately $60.4 billion annually in the U.S., encompassing property damage, health expenses, and productivity losses [2]. The implementation of a drowsiness detection system that alerts and encourages drivers to take breaks would greatly enhance vehicle safety and significantly reduce casualties.

Furthermore, the integration of emotion analysis into the system allows for a more personalized in-cabin experience. This feature could be especially appealing to luxury car manufacturers, as it offers a unique selling point to target specific customer segments.

# Approach

The project is divided into three main parts. The first part focuses on drowsiness detection, utilizing libraries such as SciPy, Imutils, Dlib, and OpenCV. The selected approach involves the use of the eye aspect ratio, which measures the openness of the driver's eyes, to determine drowsiness. The system continuously monitors the eye aspect ratio and triggers an alert when the value falls below a certain threshold, indicating that the driver's eyes are closed or partially closed.

The second part of the project involves emotion detection. The Deepface library, which incorporates state-of-the-art models like VGG-Face, Google FaceNet, and Dlib, is employed for facial attribute analysis, specifically for predicting emotions such as anger, fear, neutral, sadness, disgust, happiness, and surprise. The Convolutional Neural Network (CNN) architecture provided by Deepface is used to analyze facial expressions and determine the user's current emotion.

In the third part, the drowsiness detection and emotion analysis components are combined to create the final code. The system provides an alert when the driver is feeling drowsy and also detects and prints out the emotion being experienced.

# Transfer Learning and Pre-trained Models

To tackle the resource-intensive nature of neural network models, the project utilizes transfer learning and pre-trained models. Transfer learning enables the use of models pre-trained by others for similar problems, reducing the need to train models from scratch. This approach is particularly useful when dealing with tasks like image or voice recognition, where complex neural networks require significant computational resources.

Pre-trained models refer to models already trained to solve similar problems. Instead of building a model from scratch, these pre-trained models serve as starting points, saving substantial time and effort. However, careful consideration must be given to selecting the most appropriate pre-trained model for a specific problem. If the pre-trained model's training data and problem scope significantly differ from the current problem, the accuracy of predictions may be compromised.

# Dependencies and Libraries Used

- OpenCV: An open-source computer vision and machine learning software library used for various computer vision applications.
- Imutils: A package providing a series of convenience functions to make basic image processing functions such as translation, rotation, resizing, skeletonization, and displaying Matplotlib images easier with OpenCV.
- Keras: A high-level neural networks API, written in Python and capable of running on top of TensorFlow, CNTK, or Theano. It allows for easy and fast prototyping.
- DeepFace: A Python wrapper for deep learning-based face recognition models from famous frameworks inside, including VGG-Face, Google FaceNet, OpenFace, Facebook DeepFace, and DeepID.
- HaarCascade: A machine learning object detection method used to identify objects in images or video. Particularly, it's popular for face detection.
- TensorFlow: An open-source software library for dataflow and differentiable programming across a range of tasks, widely used for machine learning applications such as neural networks.
