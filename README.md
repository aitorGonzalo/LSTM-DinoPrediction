🦖 Dinosaur Name Generator with LSTM
📌 Project Overview

This project implements a character-level LSTM neural network to generate new dinosaur names based on a dataset of real dinosaur names.

The workflow includes:

Data preprocessing: cleaning names, building a character vocabulary, and preparing input/output sequences.

Model design: an LSTM network with an embedding layer, tuned using Keras Tuner for hyperparameter optimization.

Training: supervised learning with categorical crossentropy loss.

Name generation: using a trained model to predict character sequences and create new dinosaur names.

Evaluation: comparing generated names with real ones using similarity metrics.

⚙️ Tech Stack

Python 3

TensorFlow / Keras

Keras Tuner

Pandas / NumPy

Matplotlib

Difflib (SequenceMatcher)

🚀 How It Works

Load the dataset (dinosaur.csv) containing dinosaur names.

Create a character vocabulary and convert names into sequences.

Train an LSTM model to predict the next character given a sequence of previous characters.

Generate new dinosaur names by sampling predictions iteratively.

Compare generated names to real ones with a similarity score.

📊 Results

Example output after training: