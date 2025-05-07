Image Caption Generator

    A deep learning project that automatically generates captions for images using a Convolutional Neural Network (CNN) as an encoder and a Long Short-Term Memory (LSTM) network as a decoder.

Overview

    This project aims to generate human-like captions for images by combining visual feature extraction (using CNN) and sequence modeling (using LSTM).
    It demonstrates a full pipeline including data preprocessing, model training, evaluation with BLEU score, and inference on new images.

Architecture

    Encoder: Pre-trained VGG16 CNN to extract image features.
    Decoder: LSTM network to generate captions based on the extracted features.
    Loss Function: Categorical Cross-Entropy
    Optimizer: Adam

Dataset

    Dataset Used: , Flickr8k
    Each image has 5 associated textual captions.

Evaluation

    After training, evaluate the model performance:
    BLEU Score is used to measure the similarity between generated and ground-truth captions.

Results

    Here are some examples of generated captions:
    Image	Generated Caption
    "A dog is running across a field"
    "A man is riding a bicycle on a street"
    "A child is playing with a ball"

Future Work

    Upgrade the model to a Transformer-based Caption Generator (e.g., ViT + Transformer Decoder).
    Improve the beam search decoding method for better caption quality.
    Deploy as a full web application using Streamlit or Gradio.
    Experiment with reinforcement learning to optimize captions.