💬 Movie Review Sentiment Classification
📌 Overview

This project performs sentiment analysis on movie reviews using the IMDb dataset. The goal is to classify reviews as positive or negative based on their textual content using machine learning and deep learning models.

📂 Dataset

The dataset consists of 50,000 movie reviews, equally divided into:

Positive reviews → 25,000
Negative reviews → 25,000

Each review is labeled to indicate its sentiment.

❓ Why Sentiment Analysis?

Understanding user opinions from text data is important for:

Customer feedback analysis
Product and movie reviews
Social media monitoring
Decision-making systems
⚙️ Data Preprocessing

To improve model performance, the text data undergoes:

Removal of HTML tags and special characters
Stopword removal
Elimination of single-character noise
Normalization of whitespace
🧠 Text Representation
1. Tokenization
Converts text into sequences of numbers
Assigns a unique index to each word
2. Padding
Ensures all sequences have the same length
Maintains uniform input size
3. Word Embeddings (GloVe)
Uses pre-trained embeddings
Captures semantic meaning of words
Improves model accuracy
🤖 Models Implemented
1. Feedforward Neural Network (FNN)
Uses dense layers
Fast but less effective for sequential data
2. Convolutional Neural Network (CNN)
Captures local patterns in text
Identifies important phrases
3. Long Short-Term Memory (LSTM)
Handles sequential dependencies
Best for understanding context in text
📊 Training & Results
Models trained for 10 epochs
Performance evaluated using accuracy

👉 Observation:
LSTM achieved the highest accuracy due to its ability to capture long-term dependencies in text.

🛠️ Technologies Used
Python
NumPy
Pandas
NLTK
TensorFlow
Keras
Scikit-learn
💾 How to Run
Clone the repository
git clone <repository-link>
Navigate to project folder
cd project-folder
Install dependencies
pip install -r requirements.txt
Run the project
python main.py
🎯 Applications
Movie and product review analysis
Social media sentiment tracking
Customer feedback systems
Opinion mining
🔮 Future Improvements
Use advanced models like BERT / Transformers
Hyperparameter tuning
Add evaluation metrics (F1-score, Precision, Recall)
📜 License

This project is licensed under the MIT License
