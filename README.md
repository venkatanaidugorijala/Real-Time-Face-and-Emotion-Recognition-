# Real-Time-Face-and-Emotion-Recognition
Leveraging Deep Learning and OpenCV for Enhanced Accuracy
# Datasets:
# Face Dataset: (not included in the files)
Custom dataset collected using a webcam for 400 grayscale images per person.

# Emotion Dataset:(Pre trained model uploaded)
Used a publicly available dataset with 7 emotion classes have 35,000 images: Angry, Disgust, Fear, Happy, Neutral, Sad, and Surprise.
Training set: 28,821 images across 7 classes.
Testing set: 7,066 images across 7 classes.

# Data Split:
Both datasets were split into 80% for training and 20% for testing.

# Data Preprocessing for Facial Recognition
Face Detection
Grayscale Conversion
Resizing
Normalization

# Data Preprocessing for Emotion Detection​
Emotion Detection
Grayscale Conversion
Resizing
Normalization
Class Label Encoding

# Facial Recognition – CNN
1.Input Layer:
Grayscale images of 100x100 pixels serve as input.

2.Feature Extraction:
Convolutional Layers apply filters to extract distinctive facial features, such as the shape of eyes, nose, and mouth.
ReLU Activation introduces non-linearity to capture complex patterns.
MaxPooling reduces spatial dimensions, retaining only the most critical features

3.Classification:
Flattened feature maps are passed to Dense Layers, which map the features to individual identity labels.
The final layer uses Softmax to produce probabilities for each identity.

# Emotion Detection - CNN
1.Input Layer:
Grayscale images of 48x48 pixels are used.

2.Feature Extraction:
Convolutional layers focus on subtle patterns, such as eyebrow movement and mouth curvature, to identify emotional expressions.
ReLU and MaxPooling are applied, similar to facial recognition, to extract and compress essential features.

3.Classification:
Flattened feature maps are processed by Dense Layers to map features to 7 emotion categories.
The output layer uses Softmax to generate probabilities for each emotion, with the highest probability representing the detected emotion.

# Summary and Future Work
Achievements:
Successfully implemented a real-time, dual-function recognition system.
By using different datasets, the system became more flexible and accurate.

Future Directions:
Expand datasets to include diverse demographics.
Explore multi-model inputs like speech or gestures

