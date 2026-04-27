# 🧠 Next Word Prediction using LSTM

A simple deep learning project that predicts the next word in a sequence using an LSTM-based neural network. Built as a hands-on exploration of NLP sequence modeling and text generation.

---

## 🚀 Overview

This project trains a Long Short-Term Memory (LSTM) model on a text corpus to learn word patterns and predict the most probable next word given an input sequence.

Example:
**Input:** "I love eating"
**Output:** "pizza" 🍕

---

## 🛠️ Features

* Text preprocessing and tokenization
* Sequence generation using sliding window
* LSTM-based model for sequence prediction
* Training pipeline with loss visualization
* Interactive next-word prediction
* Lightweight and easy to extend

---

## 📂 Project Structure

```
├── data/                # Input text dataset
├── models/              # Saved trained models
├── notebooks/           # (Optional) Experimentation notebooks
├── src/
│   ├── preprocess.py    # Text cleaning & tokenization
│   ├── train.py         # Model training pipeline
│   ├── model.py         # LSTM architecture
│   └── predict.py       # Inference script
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/next-word-lstm.git
cd next-word-lstm
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 📊 How It Works

1. **Text Preprocessing**

   * Lowercasing
   * Tokenization
   * Vocabulary creation

2. **Sequence Creation**

   * Convert text into input-output pairs
   * Example:

     ```
     Input:  "I love"
     Target: "eating"
     ```

3. **Model Architecture**

   * Embedding layer
   * LSTM layers
   * Dense output layer with softmax

4. **Training**

   * Loss: Categorical Crossentropy
   * Optimizer: Adam

---

## 🏋️ Training the Model

```bash
python src/train.py
```

This will:

* Train the LSTM model
* Save the trained weights in `/models`

---

## 🔮 Making Predictions

```bash
python src/predict.py
```

Or use it interactively:

```python
predict_next_word("I love eating")
```

---

## 📈 Example Output

```
Input:  "Deep learning is"
Output: "fun"
```

---

## 📦 Requirements

* Python 3.8+
* TensorFlow / Keras
* NumPy
* Pandas (optional)

---

## 💡 Future Improvements

* Add GRU / Transformer models
* Beam search for better predictions
* Deploy as a web app (Streamlit / Flask)
* Support for larger datasets

---

## 🤝 Contributing

Pull requests are welcome. If you’ve got ideas to improve predictions or efficiency, go for it.

---
