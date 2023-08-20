This repository contains multiple machine learning models designed to predict treatment charges. The models utilize various techniques for text pre-processing and employ different architectures to achieve accurate predictions.

# Introduction

The goal of this project is to develop machine learning models capable of accurately predicting the charges of medical treatments based on textual information. The models have been trained and evaluated using various techniques to achieve high performance in terms of accuracy and validation scores.
Text Pre-Processing

# The text pre-processing pipeline involves the following steps:

   - Tokenization: The input text data is split into individual words (tokens) to create a meaningful representation for the models.

   - Text Encoding: Tokens are encoded into numerical values to be fed into the models. This encoding process helps in representing text data in a format understandable by machine learning algorithms.

   - Padding: The encoded sequences are padded to ensure uniform length, which is necessary for training the models on batches of data.

   - One-Hot Encoding: In some models, one-hot encoding is used to further represent categorical data, such as word indices, to be used as input.

# Models
## RNN Model

    Accuracy: 0.658

The RNN (Recurrent Neural Network) model is designed to capture sequential patterns in the text data. It uses recurrent layers to maintain memory of previous tokens and is suitable for tasks involving sequential data like text.

## Transfer Learning RNN

    Validation Score: 1.057
    Accuracy: 0.678

The Transfer Learning RNN leverages pre-trained embeddings to enhance its performance. It utilizes embeddings learned from a different task or dataset and fine-tunes them for the specific task of predicting treatment charges.

## Hybrid Approach (Pre-trained Embeddings with Embeddings Learned on the Fly)

    Validation Score: 2.669
    Accuracy: 0.626

The hybrid approach combines the strengths of pre-trained embeddings and embeddings learned on the fly. This approach aims to capture both general and task-specific information from the text data, potentially leading to improved predictions.


Please note that the accuracy and validation scores mentioned are based on the provided dataset and training settings.