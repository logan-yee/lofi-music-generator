# AI Lofi Music Generator 🎵

Harness the power of neural networks to generate soothing lofi beats. Model is trained using a lofi music dataset. 

## Overview

This project uses a deep learning model to understand the patterns in MIDI music files and generate new, original lofi tracks. It's built using the Keras library and processes music data with the `music21` toolkit.

## Features

- **Training on Custom Data**: Feed the model with your collection of MIDI files and let it learn the essence of your favorite lofi tracks.
- **MIDI File Generation**: Once trained, the model can produce new MIDI files that you can listen to or further process.
- **Flexible Neural Network Architecture**: The LSTM-based deep neural network can capture complex temporal dependencies in music data.

## Dependencies

- numpy
- pickle
- music21
- keras

## How to Run

1. Ensure you have all the dependencies installed.
2. Place your collection of MIDI files in the `files` directory.
3. Run the training script to train the model on your data.
4. Once trained, run the generation script to produce a new MIDI file.
5. Enjoy your AI-generated lofi track!

## Model Architecture

- **LSTM Layers**: The model uses Long Short-Term Memory (LSTM) layers to capture the temporal dependencies in music data.
- **Dense & Dropout Layers**: Dense layers allow the model to learn complex representations, while dropout layers prevent overfitting.
- **Activation & Batch Normalization**: Activation functions introduce non-linearity, and batch normalization helps in faster and more stable training.

## Data Processing

- MIDI files are parsed and processed using the `music21` toolkit.
- Notes and chords are extracted and converted into a format suitable for training the neural network.
- The processed data is then used to train the model, which learns the patterns and structures in the music.
