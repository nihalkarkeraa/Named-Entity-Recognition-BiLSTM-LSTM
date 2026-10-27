# Named Entity Recognition (NER) using BiLSTM-LSTM

## Abstract

Named Entity Recognition (NER), also known as entity recognition or entity extraction, is a Natural Language Processing (NLP) technique used to identify and classify named entities in text into predefined categories. These entities may include people, organizations, locations, dates, monetary values, and other meaningful information.

This project implements a Named Entity Recognition system using a deep learning architecture based on Bidirectional Long Short-Term Memory (BiLSTM) and Long Short-Term Memory (LSTM) networks. The model processes text sequences and predicts entity tags for individual words using contextual information.

NER can help extract important information from large volumes of textual data and is useful in applications such as information retrieval, document processing, customer support, and data analysis.

## Motivation

The motivation behind this project is to understand and implement a deep learning-based approach for automatically identifying named entities in text. Large amounts of unstructured textual data are generated across various industries, making manual extraction of relevant information time-consuming.

By implementing a BiLSTM-LSTM model, this project explores how neural networks can learn contextual relationships between words and classify them into appropriate entity categories. The project also provides practical experience in Natural Language Processing, text preprocessing, sequence modeling, and deep learning.

## Limitations of Existing Methods

Traditional rule-based NER systems depend on manually defined rules and linguistic patterns. Although these approaches can work well for specific applications, they may struggle with unfamiliar names, variations in writing, and complex sentence structures.

General-purpose pretrained NER models may also misclassify unfamiliar names or entities when the input differs from their training data. Machine learning approaches depend on the quality and diversity of annotated datasets, while deep learning models may require sufficient training data and computational resources to achieve good performance.

These limitations motivate the exploration of deep learning architectures that use contextual information to identify and classify entities.

## Proposed Method with Architecture / Flow Diagram

The proposed system uses a BiLSTM-LSTM architecture to perform Named Entity Recognition. The input text is preprocessed, tokenized, and converted into numerical sequences. The model uses an embedding layer to represent words as vectors, followed by a bidirectional LSTM layer and an additional LSTM layer to learn contextual information.

A TimeDistributed Dense layer with softmax activation predicts an entity tag for each token in the sequence.

### System Workflow

1. Dataset acquisition
2. Data preprocessing and tokenization
3. Mapping words and entity tags to numerical indices
4. Sequence grouping and padding
5. Building the BiLSTM-LSTM model
6. Training the model
7. Testing and evaluating the model
8. Visualizing and interpreting named entities

### Model Architecture

Input Text → Tokenization and Preprocessing → Word Embedding → Bidirectional LSTM → LSTM → TimeDistributed Dense Layer → Entity Tag Predictions

*Insert your model architecture diagram or workflow diagram here.*

## Modules with Description

### 1. Acquiring Dataset

The dataset is loaded into the Python environment for processing and model development. It contains text tokens and their corresponding entity labels.

### 2. Extracting Mappings: Features and Labels

Words and entity tags are converted into numerical indices. These mappings allow the neural network to process textual input and learn the relationship between words and their corresponding labels.

### 3. Extracting Data Sequentially

The dataset is grouped by sentence, and words and tags are organized into sequences. Padding is applied where necessary to make sequences compatible with batch-based model training.

### 4. Identifying the Best-Fit Model

A BiLSTM-LSTM neural network is constructed. The embedding layer represents words numerically, while recurrent layers learn contextual relationships across sequences.

### 5. Training the Model

The model is trained using the prepared token sequences and their corresponding entity tags. The training process adjusts model parameters to reduce prediction error.

### 6. Testing the Model

The trained model can be used to predict entity labels for input sequences that were not used during training.

### 7. Evaluating and Improving the Model

Model performance can be assessed using training and validation loss, accuracy, and suitable NER evaluation metrics such as precision, recall, and F1-score. The results can help identify opportunities for improvement.

## Screenshots

Include screenshots of the following:

- Dataset and preprocessing output
- Model architecture and layer summary
- Training progress and validation metrics
- Named entity recognition output
- Final evaluation results

*Insert screenshots from your actual implementation here.*

## Conclusion

This project demonstrates the implementation of a deep learning-based Named Entity Recognition system using a BiLSTM-LSTM architecture. The system processes text sequences and predicts entity labels for individual tokens.

The project provides practical experience in NLP, data preprocessing, sequence modeling, and neural network training. Future improvements may include using larger and more diverse datasets, tuning hyperparameters, applying suitable evaluation metrics, and experimenting with more advanced architectures.

## Contributors

- Nihal Karkera
- Sanjay Moolya
- Anurudh K
- Shrusti Shiny
- Vidyashree

## Institution

Srinivas University Institute of Engineering and Technology

## Project Domain

Natural Language Processing (NLP) and Deep Learning
