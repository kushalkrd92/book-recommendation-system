# 📚 Book Recommendation System

A machine learning–based Book Recommendation System that suggests similar books based on user input using collaborative filtering techniques. The system analyzes user–item interactions and computes similarity scores to generate personalized recommendations 

---

## 🚀 Features

* 📖 Recommend top 10 similar books based on selected title
* 🔎 Collaborative filtering using similarity matrix
* 📊 Popular books display on homepage
* ⚡ Fast recommendation using precomputed similarity scores
* 🌐 Web interface built using Flask

---

## 🧠 How It Works

1. A user–item pivot table is created from book ratings data.
2. Cosine similarity is computed between books.
3. Similarity scores are stored using Pickle for faster inference.
4. When a user selects a book:

   * The system retrieves its index in the pivot table
   * Finds the most similar books using the similarity matrix
   * Returns the top recommendations dynamically 

---

## 🛠 Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **Flask**
* **Pickle**
* **HTML (Jinja Templates)**

Project dependencies are listed in `requirements.txt` 

---

## 💻 Installation

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/book-recommendation-system.git
cd book-recommendation-system
```

---

### 2️⃣ Create Virtual Environment (Recommended)

```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # Mac/Linux
```

---

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

Dependencies are predefined in `requirements.txt` 

---

## ▶️ Usage

Run the Flask application:

```bash
python app.py
```

Then open your browser and go to:

```
http://127.0.0.1:5000/
```

---

## 📂 Project Structure

```
│── app.py
│── popular.pkl
│── books.pkl
│── pt.pkl
│── similarity_scores.pkl
│── templates/
│     ├── index.html
│     └── recommend.html
│── requirements.txt
```

---

## 📌 Example Workflow

1. Open homepage to view popular books
2. Navigate to recommendation page
3. Enter a book title
4. Receive top 10 similar book recommendations

---
