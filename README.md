# 🎬🎵📚 Smart Recommender System with Vectorization

This project is a **recommendation system** that suggests **movies**, **music**, **TV shows**, and **books** using **vectorization techniques**. It is developed using **JavaScript** for both the frontend and backend, while the **core recommendation engine is implemented in Python**. All datasets are custom-created and structured in JSON format with domain-specific features.

## 🚀 Features

- 🔍 Content-based recommendation engine using vector similarity
- 🧠 Implemented in Python with cosine similarity
- 🌐 Interactive frontend built with vanilla JavaScript
- 💾 Custom JSON datasets for each domain (movies, music, series, books)
- 🔄 Easy-to-extend architecture for adding new content types

## 📁 Dataset

All the data used in this project is created manually and made publicly available on Kaggle:

👉 [View the Dataset on Kaggle](https://www.kaggle.com/datasets/cihanivit/book-data-set/data)

The dataset contains structured JSON files for:
- `books.json`
- `movies.json`
- `music.json`
- `series.json`

Each JSON file is tailored to the content it represents, with features used in the vectorization process.

## 🧩 Technologies Used

| Component   | Technology      |
|------------|-----------------|
| Frontend   | JavaScript, HTML, CSS |
| Backend    | JavaScript (Node.js) |
| Recommendation Engine | Python (scikit-learn, numpy) |
| Data Format | JSON |
| Dataset Hosting | Kaggle |

## ⚙️ Installation

1. **Clone the repository:**
```bash
git clone https://github.com/cihanivit/media-recommender.git
cd media-recommender
```

2. **Install dependencies:**
```bash
# For Python part
cd recommender-engine
pip install -r requirements.txt

# For frontend/backend
cd ../frontend
npm install
```

3. **Run the Python recommendation server (Flask/FastAPI/etc.):**
```bash
python app.py
```

4. **Run the frontend/backend:**
```bash
# For simple development server
npx http-server .
```

## 💡 How It Works

1. User selects a favorite item (e.g., a book or movie).
2. The selected item's vector representation is sent to the Python backend.
3. Backend calculates cosine similarity with other items in the dataset.
4. A ranked list of similar items is returned and shown to the user.

## 🧪 Example JSON Entry (Book)

```json
  {
      "name": "The Metamorphosis",
      "rating": 4.6,
      "genre_1": "Classic",
      "genre_2": "Psychology",
      "description": "A man transforms into an insect, facing alienation and despair.",
      "writer": "Franz Kafka",
      "ID": 7
  }
```
