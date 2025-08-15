# Push-up Counting Model with Computer Vision

This project uses machine learning and computer vision to count push-ups in real-time by detecting and classifying body poses. 
It leverages Google's Mediapipe for pose estimation and a Random Forest Classifier to detect push-up repetitions.

## Features:
- Real-time push-up rep counting.
- Voice feedback when a rep is counted or posture correction is needed.
- Model trained on custom dataset with pose landmarks.
- Can be tested on videos or webcam footage.

## Technologies Used:
- **Python 3.x**
- **Mediapipe**: For pose detection.
- **OpenCV**: For video processing.
- **scikit-learn**: For the Random Forest Classifier.
- **pyttsx3**: For text-to-speech feedback.
- **pygame**: For background music (optional).

## Files in the Repository:
- `pose_landmarks_dataset.csv`: Dataset containing the pose landmarks for push-ups.
- `pose_pushup_classifier.pkl`: The trained Random Forest model.
- `main.ipynb`: Jupyter Notebook with code for testing the model.

## How to Run:
1. **Clone the repository**:
   git clone https://github.com/rakibahmedhimel/pushup-repetition-count.git
2. **Install the required dependencies:**
   pip install -r requirements.txt
3. **Test the model:**
   Open the main.ipynb file and run the code in Jupyter Notebook to test the model with your video or webcam footage.
   If you prefer to run it outside Jupyter, you can use the main.py script (if you create one based on the notebook).


## Model Overview:
The model is trained on pose landmarks captured during push-ups, using Mediapipe to detect body keypoints. 
The classifier is trained to recognize "up", "down", and "wrong" postures, allowing for accurate rep counting.

## Demo Video:
Check out the demo video in asset folder to see how the model performs in real-time.

## License:
All rights reserved. No redistribution or modification without permission.
