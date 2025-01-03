
# Toxicity Detection in Comments using LSTM

This project implements a model for detecting toxic comments in online platforms using **LSTM (Long Short-Term Memory)** networks. The goal is to classify comments as either "toxic" or "non-toxic" based on their content. Toxic comments often include hate speech, insults, or offensive language, and detecting them is critical for ensuring a positive online environment.

## Objective

The primary objective of this project is to build a machine learning model that can automatically classify comments as either toxic or non-toxic. The model is based on an **LSTM** architecture, which is well-suited for natural language processing (NLP) tasks involving sequences like text.

## Dataset

This project uses a dataset containing labeled comments, where each comment is marked as either toxic or non-toxic. The dataset is pre-processed to clean and tokenize the text data for training the model.

The dataset includes:
- **Toxic comments**: Comments that contain hate speech, abuse, or offensive language.
- **Non-toxic comments**: Comments that are neutral and do not contain harmful language.

The dataset is available from Kaggle's Toxic Comment Classification Challenge

## Model Architecture

The model is built using **LSTM** (Long Short-Term Memory) networks, which are a type of Recurrent Neural Network (RNN) that can capture long-term dependencies in text sequences. The architecture consists of the following layers:

1. **Embedding Layer**: Converts each word in the input text into a dense vector representation.
2. **Bidirectional LSTM Layer**: The LSTM layer is bidirectional, meaning it processes the text sequence in both forward and backward directions to capture contextual information.
3. **Dense Layers**: Fully connected layers to process the features extracted by the LSTM.
4. **Output Layer**: A sigmoid output layer that produces a probability of the comment being toxic (0 or 1).

### LSTM Model Architecture Overview:
- **Input**: Text comments (tokenized and padded)
- **Embedding Layer**: Maps words to dense vectors
- **Bidirectional LSTM Layer**: Extracts sequential features from the text
- **Dense Layers**: Fully connected layers with ReLU activation
- **Output Layer**: Sigmoid activation function for binary classification (toxic vs non-toxic)

