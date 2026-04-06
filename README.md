Movie Review Sentiment Classification
Project Overview

This project performs sentiment analysis on movie reviews using the IMDb dataset. The objective is to build machine learning models capable of classifying reviews as positive or negative based on textual content.

Dataset Details

The dataset contains 50,000 labeled movie reviews, evenly split:

Sentiment	Samples
Positive	25,000
Negative	25,000

Source: IMDb Movie Reviews Dataset (Kaggle)

Data Cleaning & Preprocessing

To improve model performance, the text data is cleaned and normalized through several steps:

Removing HTML tags and unwanted symbols
Eliminating common stopwords
Filtering out single-character noise
Normalizing extra whitespace

These steps help in reducing noise and improving feature quality.

Text Representation
Tokenization

Text is converted into sequences of integers using a tokenizer. Each word is mapped to a unique index.

Padding

Since reviews vary in length, sequences are padded to a fixed size (e.g., 100 words) to ensure uniform input for models.

Word Embeddings (GloVe)

Pre-trained GloVe embeddings are used to represent words as dense vectors. This allows the model to:

Understand semantic relationships
Improve generalization
Capture contextual meaning
Models Implemented

Three different models are used to compare performance:

1. Feedforward Neural Network
Basic dense layers
Fast but less effective for sequence data
2. Convolutional Neural Network (CNN)
Uses 1D convolution layers
Captures local text patterns and phrases
3. Long Short-Term Memory (LSTM)
Handles sequential dependencies
Best suited for understanding context in sentences
Training & Results
Models are trained for 10 epochs
Performance is evaluated using accuracy

👉 Observation:
The LSTM model achieves the highest accuracy due to its ability to capture long-term dependencies in text.

Requirements

Install the following libraries before running the project:

Python 3.x
NumPy
Pandas
NLTK
TensorFlow
Keras
Scikit-learn

Also, download GloVe embeddings from the official source.

How to Run
git clone <repository-link>
cd project-folder
pip install -r requirements.txt
python main.py
Future Improvements
Use Transformer models (like BERT)
Hyperparameter tuning
Add more evaluation metrics (F1-score, Precision, Recall)
License

This project is licensed under the MIT License.

Contributions

Contributions are welcome! Feel free to fork the repo and submit a pull request.
