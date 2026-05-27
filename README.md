# 🎬 IMDB Movie Review Sentiment Analysis

A deep learning web app that classifies movie reviews as **Positive** or **Negative** using a Simple RNN model trained on the IMDB dataset — built with TensorFlow and deployed via Streamlit. Fully Dockerized for easy deployment.

---

## 🚀 Demo

Enter any movie review and the model will instantly predict whether the sentiment is **Positive** or **Negative** along with a confidence score.

---

## 🧠 How It Works

1. User enters a movie review in the Streamlit app
2. The text is preprocessed and tokenized using the IMDB word index
3. The sequence is padded to a fixed length of 500
4. A pre-trained Simple RNN model predicts the sentiment
5. Result is displayed with a confidence score

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.10 | Core language |
| TensorFlow / Keras | RNN model training & inference |
| Streamlit | Web app UI |
| NumPy | Numerical processing |
| Docker | Containerization |

---

## 📁 Project Structure

```
simple_rnn_imdb/
│
├── main.py                  # Streamlit app
├── simple_rnn_imdb.h5       # Pre-trained RNN model
├── requirements.txt         # Python dependencies
├── Dockerfile               # Docker configuration
├── .dockerignore            # Docker ignore rules
├── simplernn.ipynb          # Model training notebook
├── prediction.ipynb         # Prediction experiments
└── embedding.ipynb          # Embedding experiments
```

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/imdb-sentiment-analysis.git
cd imdb-sentiment-analysis
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
streamlit run main.py
```

Open your browser at **http://localhost:8501**

---

## 🐳 Run with Docker

```bash
# Build the image
docker build -t imdb-sentiment-analysis .

# Run the container
docker run -p 8501:8501 imdb-sentiment-analysis
```

Open your browser at **http://localhost:8501**

---

## 📊 Model Details

- **Architecture:** Simple RNN
- **Dataset:** IMDB Movie Reviews (50,000 reviews)
- **Vocabulary Size:** 10,000 words
- **Max Sequence Length:** 500
- **Activation:** ReLU
- **Task:** Binary Sentiment Classification (Positive / Negative)

---

## 📦 Requirements

```
tensorflow==2.15.0
pandas
numpy
scikit-learn
tensorboard
matplotlib
streamlit
scikeras
```

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

Made with ❤️ — feel free to fork, star ⭐, and contribute!
