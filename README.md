# Fingerprint-Biometric-Authentication

This project implements a fingerprint-based biometric authentication system using deep learning. It leverages Siamese networks to perform user verification by learning embeddings for fingerprints and comparing them for authentication.

- Overview
    The system supports two approaches:
  
      1- Triplet Loss-based Siamese Network – learns embeddings from anchor, positive, and negative samples.
  
      2- Pairwise Binary Classification Siamese Network – predicts similarity probability between pairs of images.
  
    The workflow includes image preprocessing, triplet/pair generation, model training, and biometric verification. The system can visualize anchor, positive, and negative images and evaluate performance on unseen       test samples.

-  Dataset

    - Fingerprint bitmap images (.bmp) stored in a zip file.

    - Labels are extracted from filenames.

    - Preprocessing includes Gaussian blur, histogram equalization, and normalization.

- Features

  - Automatic extraction and preprocessing of dataset

  -Training of Triplet Loss-based and Pairwise Siamese networks
  
  - Biometric verification using stored embeddings
  
  - Evaluation using accuracy, precision, recall, F1-score, ROC-AUC, and distance ratio
  
  - Visualizations for training and testing samples
 
- Model Architecture

  - Convolutional layers with pooling and batch normalization

  - Dense layers for embedding generation

  - Triplet Loss or binary classification output depending on the model

  - Euclidean distance or similarity threshold used for authentication
 
- Evaluation

    Both models are evaluated using: accuracy, precision, recall, F1-score, ROC-AUC, and distance ratio (for the Triplet model). Visual plots for training vs. validation loss provide insights into model performance.

- Results

    The models demonstrate effective fingerprint verification, with the Triplet model providing embedding-based comparison and the Pairwise model providing similarity probability-based authentication.
