# Emotion Recognition

### Project Definition:
Classifying a person’s emotion, from a list of 7 emotions, using their facial expression. Downloaded face images 
[Kaggle Dataset](https://www.kaggle.com/c/facial-keypoints-detector) that came as a csv file with grayscale images converted into binary, and used Haar Cascade Frontal Face code to detect faces in live video feed.

**Emotions:**
- anger
- disgust
- fear
- happy
- sad
- surprise
- neutral

### Models & Metrics:
1) 4-layer model using relu and softmax --> 0.09 validation accuracy 
2) 6-layer CNN model of tanh, MaxPooling2D, and softmax --> F1-score = 0.45
3) 6-layer CNN model of tanh, MaxPooling2D, and softmax, normalized data, batch-size = 10 early callback --> F1-score = 0.78
4) Added one more tanh layer to last model --> F1-score = 0.78
5) VGG16 with 2 tanh layers and softmax output layer --> F1-score = 0.88
6) VGG19 with 2 tanh layers and softmax output layer --> F1-score = 0.78

