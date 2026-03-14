# Next Word Prediction using LSTM (Streamlit App)

This project builds a **Next Word Prediction Web Application** using an **LSTM (Long Short-Term Memory) neural network** trained on **Shakespeare's Hamlet text** from the NLTK Gutenberg corpus.

The trained deep learning model learns language patterns from the dataset and predicts the most likely **next word** given an input sequence.

The application is deployed locally using **Streamlit**, allowing users to interactively test the model.

---

# Project Overview

Natural language processing models can learn patterns in sequences of words and predict the next probable word in a sentence.

In this project:

1. Text data is collected from the **NLTK Gutenberg corpus**
2. The dataset is preprocessed and tokenized
3. Training sequences are created
4. An **LSTM neural network** is trained to learn word relationships
5. The trained model is saved
6. A **Streamlit web application** is built to interact with the model

Users can input a sequence of words and the model will predict the **next word**.

---

# Example

Input

```
To be or not to be
```

Output

```
against
```

The model predicts the most likely next word based on patterns learned from Shakespeare's text.

---

# Tech Stack

This project uses the following technologies:

* Python
* TensorFlow / Keras
* NumPy
* NLTK
* Scikit-learn
* Streamlit
* Jupyter Notebook

---

# Dataset

The dataset used in this project is **Shakespeare's Hamlet** from the **NLTK Gutenberg Corpus**.

The text is processed and converted into numerical sequences for training the LSTM model.

Dataset source:

https://www.nltk.org/book/ch02.html

---

# Model Architecture

The deep learning model consists of the following layers:

Embedding Layer
LSTM Layer
Dropout Layer
Dense Output Layer

Model Summary

Total Parameters: **860,970**
Trainable Parameters: **860,970**
Non-Trainable Parameters: **0**

---

# Project Structure

```
LSTM-RNN-Next-Word-Predictor
│
├── app.py
├── experiments.ipynb
├── next_word_lstm.h5
├── tokenizer.pickle
├── hamlet.txt
├── requirements.txt
├── README.md
└── .gitignore
```

Description of files:

app.py
Streamlit web application that loads the trained model and predicts the next word.

experiments.ipynb
Jupyter Notebook used for data preprocessing, model training, and experimentation.

next_word_lstm.h5
Saved trained LSTM model.

tokenizer.pickle
Saved tokenizer used during model training.

hamlet.txt
Training dataset extracted from the Gutenberg corpus.

requirements.txt
List of Python dependencies required to run the project.

README.md
Project documentation.

---

# How to Run the Project Locally

## 1. Clone the repository

```
git clone https://github.com/YOUR_USERNAME/lstm-next-word-predictor.git
cd lstm-next-word-predictor
```

---

## 2. Create a virtual environment

Mac / Linux

```
python3 -m venv venv
source venv/bin/activate
```

Windows

```
python -m venv venv
venv\Scripts\activate
```

---

## 3. Install the required dependencies

```
pip install -r requirements.txt
```

---

## 4. Run the Streamlit app

```
streamlit run app.py
```

---

## 5. Open the application

After running the command above, Streamlit will generate a link such as:

```
http://localhost:8501
```

Open this link in your browser.

---

# How the Prediction Works

1. User enters a sequence of words
2. The tokenizer converts the text into numerical tokens
3. The sequence is padded to match the model input size
4. The trained LSTM model predicts the next word probability
5. The most probable word is returned to the user

---

# Learning Outcomes

This project helped demonstrate several important NLP and deep learning concepts:

* Text preprocessing for NLP
* Tokenization and sequence generation
* LSTM architecture for language modeling
* Training sequence prediction models
* Saving and loading trained models
* Building ML applications using Streamlit
* Deploying machine learning models interactively

