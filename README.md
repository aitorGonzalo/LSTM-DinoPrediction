# 🦖 Dinosaur Name Generator with LSTM

## 📌 Project Overview
This project implements a character-level **LSTM neural network** to generate new dinosaur names based on a dataset of real dinosaur names.

The workflow includes:
- **Data preprocessing**: cleaning names, building a character vocabulary, and preparing input/output sequences.  
- **Model design**: an LSTM network with an embedding layer, tuned using **Keras Tuner** for hyperparameter optimization.  
- **Training**: supervised learning with categorical crossentropy loss.  
- **Name generation**: using a trained model to predict character sequences and create new dinosaur names.  
- **Evaluation**: comparing generated names with real ones using similarity metrics.  

---

## ⚙️ Tech Stack
- Python 3  
- TensorFlow / Keras  
- Keras Tuner  
- Pandas / NumPy  
- Matplotlib  
- Difflib (SequenceMatcher)  

---

## 🚀 How It Works
1. Load the dataset (`dinosaur.csv`) containing dinosaur names.  
2. Create a character vocabulary and convert names into sequences.  
3. Train an LSTM model to predict the next character given a sequence of previous characters.  
4. Generate new dinosaur names by sampling predictions iteratively.  
5. Compare generated names to real ones with a similarity score.  

---

## 📊 Results
Example output after training:

Real Name            | Generated Name       | Similarity
------------------------------------------------------------
aardonyx             | Aatasaurus           | 0.33
abelisaurus          | Abudiasaurusa        | 0.58
abrictosaurus        | Abropcosauruste      | 0.71
abrosaurus           | Abrariasauru         | 0.64
abydosaurus          | Abrosaurustas        | 0.67
...
zuniceratops         | Zurriaceratops       | 0.77
zuolong              | Zukypalti            | 0.25
zupaysaurus          | Zuroplosaurus        | 0.67
zuul                 | Zuroco               | 0.20
