🖼️ Image Caption Generator
📌 Overview

This project is an Image Caption Generator that automatically generates meaningful descriptions for images using Deep Learning. It combines Computer Vision and Natural Language Processing to understand image content and convert it into human-readable text.

✨ Features
Automatically generates captions for images
Uses deep learning models for better accuracy
Supports multiple captions per image during training
Easy to train and test with new images
Preprocessing for both images and text

🏗️ Architecture
The model follows an Encoder-Decoder architecture:
Encoder (CNN)
Extracts features from images using a pre-trained model like InceptionV3
Decoder (LSTM)
Generates captions word-by-word using extracted features
Embedding Layer
Converts words into numerical vectors
Dense Layer
Predicts the next word in the sequence

📂 Dataset – Flickr8k
We used the Flickr8k Dataset for training and testing.

Dataset Details:
Contains 8,000 images
Each image has 5 different captions
Captions describe objects, actions, and scenes in images
Preprocessing:
Images resized and normalized
Captions cleaned (lowercase, removed punctuation)
Tokenization and sequence generation
Vocabulary creation

⚙️ Technologies Used
Python
TensorFlow / Keras
NumPy
Pandas
Matplotlib

🔄 How It Works
Load and preprocess the Flickr8k dataset
Extract image features using CNN
Convert captions into sequences
Train LSTM model using image features + text data
During prediction, model generates caption word-by-word

🖼️ Example Output
Input Image: (add your image here)
Generated Caption:
👉 "A man is riding a bicycle on the road"
