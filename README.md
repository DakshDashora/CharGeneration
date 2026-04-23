# 🔤 Character-Level Text Generation using RNN

This project implements a **Character-Level Text Generator** using a **Recurrent Neural Network (RNN)** trained on the *Harry Potter* book series dataset. The model learns patterns from text and generates new sequences character by character.

Unlike word-level models, this approach:

* Learns spelling, punctuation, and writing style
* Can generate entirely new words
* Works effectively even with relatively smaller structured datasets

This project is a strong introduction to **sequence modeling and Natural Language Processing (NLP)**.

---

## 🚀 Project Overview

Text generation is a core NLP task where a model predicts the next element in a sequence.

In this project:

* Text is processed at the **character level**
* The model learns the probability of the next character
* New text is generated step-by-step using predictions

Applications include:

* Story generation
* Chatbots
* Code generation

---

## 📊 Dataset Details

### 📁 Dataset

* **Name:** Harry Potter LSTM Dataset
* **Source:** Kaggle
* **Link:** https://www.kaggle.com/datasets/moxxis/harry-potter-lstm

### 📚 Dataset Description

* Contains **all 7 Harry Potter books** in cleaned plain-text format
* Combined into a single continuous text file

### 🧹 Preprocessing Done

* Removed:

  * Formatting tags
  * Chapter headings
  * Special symbols and unnecessary characters
* Converted to clean, continuous lowercase text (if applied)

### 📏 Dataset Size

* Approximately **5+ million characters**

### 🔡 Vocabulary

* Built from **unique characters in the dataset**
* Each character is mapped to a numerical index

### 🧠 Training Format

* Input: sequence of characters
* Output: next character

Example:

* Input: `"hogwarts schoo"`
* Target: `"l"`

---

## 🧠 How It Works

1. **Data Preprocessing**

   * Convert text into numerical format
   * Create character-to-index mappings
   * Generate training sequences

2. **Model Architecture**

   * Recurrent Neural Network (RNN)
   * Learns sequential dependencies in text

3. **Training**

   * Predicts next character in sequence
   * Optimizes using loss minimization

4. **Text Generation**

   * Start with a seed string
   * Predict next characters iteratively
   * Generate continuous text

---

## 🛠️ Tech Stack

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* Jupyter Notebook

---

## 📂 Project Structure

CharGeneration/
│── TextGenerationUsingRNN.ipynb   # Main notebook
│── README.md                      # Documentation

---

## ▶️ How to Run

1. Clone the repository:
   git clone https://github.com/DakshDashora/CharGeneration.git
   cd CharGeneration

2. Install dependencies:
   pip install numpy tensorflow keras matplotlib

3. Open Jupyter Notebook:
   jupyter notebook

4. Run:
   TextGenerationUsingRNN.ipynb

---

## 📊 Example Output

Input: "harry"
Generated: "harry looked at him and said what are you doing here..."

*(Output varies based on training and randomness)*

---

## ✨ Features

* Character-level text generation
* Learns writing style from dataset
* Supports custom datasets
* Beginner-friendly implementation

---

## ⚠️ Limitations

* Requires significant training time
* May generate imperfect or incoherent text
* Basic RNN (can be improved using LSTM/GRU)

---

## 🔮 Future Improvements

* Upgrade to LSTM / GRU
* Add temperature-based sampling
* Train on larger or multiple datasets
* Deploy as a web application

---

## 🤝 Contributing

Feel free to fork this repo and improve the model!

---

## 📌 Author

Daksh Dashora

---

## ⭐ Give a Star

If you found this helpful, please ⭐ the repository!
