Next-Word Prediction Using LSTM (AI Dataset)
This project builds a simple Next-Word Prediction system using a custom AI-themed text dataset. It trains an LSTM-based deep learning model to suggest the next word based on a user’s input phrase.

📌 Features
Predicts the next word from a user-entered phrase

Shows top-5 most likely words (excluding common ones like “the”)

Trained on a clean, curated AI-based dataset

Command-line interaction (no UI framework used)

Supports reusable saved models and tokenizer

🛠 Tech Stack
Python

TensorFlow / Keras

Numpy

Tokenizer with pickle

Custom .txt dataset on Artificial Intelligence

📁 Project Structure
bash
Copy
Edit
├── next_word.py           # Main script to train and predict
├── model.h5               # Saved LSTM model
├── tokenizer.pkl          # Saved tokenizer
├── ai_dataset.txt         # AI-focused training corpus
├── requirements.txt       # List of dependencies
└── README.md              # Project description
▶️ How to Run
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the predictor

bash
Copy
Edit
python next_word.py
Example usage

markdown
Copy
Edit
Enter a phrase (or type 'exit'): artificial intelligence is
Top-5 next word suggestions:
1. transforming
2. advancing
3. evolving
4. changing
5. shaping
🧠 Model Training (if re-training is needed)
python
Copy
Edit
model.fit(X, y, epochs=30)
model.save("model.h5")

with open("tokenizer.pkl", "wb") as f:
    pickle.dump(tokenizer, f)
