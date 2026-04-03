# Facial Expression Recognition using CNN and OpenCV

## Overview

This project implements a facial emotion recognition system using a Convolutional Neural Network (CNN). The system classifies human facial expressions into multiple emotion categories based on image input.

The application uses OpenCV for image preprocessing and a Softmax classifier for multi-class emotion prediction.

---

## Key Features

* CNN-based deep learning model for emotion classification
* Image preprocessing using OpenCV
* Multi-class classification using Softmax activation
* Model persistence (JSON + H5) for reuse without retraining
* Simple GUI interface for interaction

---

## Emotion Classes

The model predicts the following emotions:

* Angry
* Disgusted
* Fearful
* Happy
* Neutral
* Sad
* Surprised

---

## Tech Stack

* Python
* TensorFlow / Keras
* OpenCV
* NumPy
* Tkinter

---

## Project Workflow

1. Load and organize dataset by emotion classes
2. Preprocess images (resize to 32×32, normalization)
3. Train CNN model on labeled data
4. Save trained model architecture and weights
5. Load model and perform emotion prediction

---

## Model Architecture

* Convolutional layers for feature extraction
* MaxPooling layers for dimensionality reduction
* Fully connected Dense layer
* Output layer with Softmax activation

---

## Training Details

* Optimizer: Adam
* Loss Function: Categorical Crossentropy
* Input Size: 32×32 RGB images
* Output: 7 emotion classes

---

## Project Structure

```id="struct_final"
facial-expression-recognition/
│
├── model/
│   ├── cnnmodel.json
│   ├── cnnmodel_weights.h5
│
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
```

---

## Installation

### Install dependencies

```bash id="install_cmd"
pip install -r requirements.txt
```

---

## Usage

```bash id="run_cmd"
python app.py
```

---

## Project Scope

This project explores multiple approaches for facial emotion recognition, including:

* PCA-based feature extraction (conceptual)
* CNN vs RNN comparison
* YOLO-based face detection (conceptual)

The final implementation uses a CNN-based model, which demonstrated better performance for image-based emotion classification.

---

## Limitations

* Uses low-resolution images (32×32)
* Basic CNN architecture
* No real-time webcam integration
* Performance depends on dataset quality

---

## Future Improvements

* Real-time emotion detection using webcam
* Integration of advanced architectures (ResNet, MobileNet)
* Improved dataset balancing and augmentation
* Deployment as a web or mobile application

---

## Author

Developed as part of an academic project and refined for practical understanding and demonstration of deep learning concepts.
