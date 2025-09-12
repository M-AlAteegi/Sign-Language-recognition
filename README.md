# Sign-Language-recognition

## Overview
This project is a **real-time sign language recognition system** built using **MediaPipe, TensorFlow/Keras, and OpenCV**.  
It collects hand landmarks, trains a Multi-Layer Perceptron (MLP) model, and performs live recognition of gestures.

The aim is to provide a lightweight solution that can run on resource-constrained devices while supporting sign language communication.

---

## Features
- Hand landmark collection with **MediaPipe**  
- CSV-based dataset (`asl_dataset.csv`)  
- Model training using **MLP neural networks** (`MLP_Training.ipynb`)  
- Real-time gesture recognition (`TheModel.ipynb`)  
- Encoders and scalers saved for reuse (`label_encoder.pkl`, `scaler.pkl`)  
- Pre-trained model provided (`asl_mlp_model.h5`)  

---

## Project Structure
├── asl_dataset.csv # Dataset of hand landmarks

├── asl_mlp_model.h5 # Trained MLP model

├── label_encoder.pkl # Label encoder for gestures

├── scaler.pkl # Scaler for normalizing data

├── LandMark_Collection.ipynb # Collect hand landmark data

├── MLP_Training.ipynb # Train the MLP model

├── TheModel.ipynb # Run real-time recognition

├── requirements.txt # Project dependencies

└── README.md # Project documentation


---

### Installation & Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/M-AlAteegi/sign-language-recognition.git
   cd sign-language-recognition

2. Install dependencies:

   pip install -r requirements.txt


3. Collect gesture data:

   jupyter notebook LandMark_Collection.ipynb


4. Train the model:

   jupyter notebook MLP_Training.ipynb


5. Run real-time recognition:

   jupyter notebook TheModel.ipynb

### Requirements

-Python 3.8+

-TensorFlow / Keras

-OpenCV

-MediaPipe

-NumPy & Pandas

-scikit-learn

(See requirements.txt for exact versions.)

### Future Work

-Expand dataset with more sign language gestures

-Add sentence-level recognition using RNNs or Transformers

-Optimize model for mobile deployment (TensorFlow Lite)

### License

This project is licensed under the MIT License.
