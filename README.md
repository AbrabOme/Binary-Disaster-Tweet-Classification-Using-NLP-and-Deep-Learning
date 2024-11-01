# Binary-Disaster-Tweet-Classification-Using-NLP-and-Deep-Learning

This project implements a deep learning model to classify tweets as either related to a disaster or not. Using advanced NLP techniques, the model leverages architectures such as Bidirectional LSTM (Bi-LSTM) and Bidirectional GRU (Bi-GRU) to achieve reliable classification. The goal is to create a robust classifier that can distinguish disaster-related tweets, aiding in emergency response scenarios.

Dataset
The dataset, sourced from a Kaggle challenge, contains tweets with binary labels indicating whether each tweet is related to a disaster or not.

Dataset Format
The dataset is in CSV format with two main columns:

text: The content of the tweet.
target: The binary label where 1 indicates a disaster-related tweet, and 0 denotes non-disaster content.
Preprocessing
Text data is tokenized and standardized using padding to ensure consistent sequence length for model input.

Model Architecture
The model architecture includes multiple layers:

Embedding Layer: Converts words into vectors, enhancing input representation.
Bidirectional LSTM and GRU Layers: Capture dependencies in the text from both directions for a nuanced understanding.
Dropout and Batch Normalization: Prevent overfitting and enhance generalization.
Fully Connected Layers: To consolidate learned features for final classification.
Results
Model Performance:

Bi-LSTM:

Precision: 0.825
Recall: 0.732
F1 Score: 0.775
Bi-GRU:

Precision: 0.832
Recall: 0.784
F1 Score: 0.807
Evaluation Metrics
A confusion matrix and classification report offer insights into the model's precision, recall, and F1-score, providing a detailed breakdown of performance across true positive, false positive, and other prediction metrics.

Future Improvements
Potential future improvements include:

Experimenting with transformer-based architectures such as BERT for improved accuracy.
Utilizing data augmentation techniques to expand and diversify the training data.
Further tuning hyperparameters to enhance model performance.
