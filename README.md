# 🎬 Movie Recommendation System

A content-based movie recommendation system built using Python, Machine Learning, FastAPI, and Streamlit. The application provides movie recommendations based on genre preferences and content similarity using TF-IDF vectorization.

## 🚀 Features

- **Movie Discovery:** Browse and explore movies.
- **Movie Search:** Search for movies using TMDB data.
- **Genre-Based Recommendations:** Discover movies based on genre preferences.
- **Content-Based Recommendations:** Get similar movie recommendations using TF-IDF and cosine similarity.
- **Movie Details:** View movie information and details.
- **Interactive Interface:** User-friendly frontend built with Streamlit.
- **REST API:** Backend services developed using FastAPI.

## 🛠️ Technologies Used

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Frontend | Streamlit |
| Backend | FastAPI, Uvicorn |
| Machine Learning | Scikit-learn, TF-IDF |
| Data Processing | Pandas, NumPy |
| API Integration | TMDB API, HTTPX, Requests |
| Data Storage | Pickle |

## 🧠 Recommendation Approach

The project implements two recommendation approaches:

### 1. Genre-Based Recommendation
Recommends movies based on selected genre preferences.

### 2. Content-Based Recommendation
Uses TF-IDF vectorization and similarity calculations to identify movies with similar content and recommend relevant titles.

## 📁 Project Structure

```text
movie-recommendation-system/
│
├── app.py                  # Streamlit frontend
├── main.py                 # FastAPI backend
│
├── df.pkl                  # Processed movie dataset
├── indices.pkl             # Movie title-index mapping
├── tfidf.pkl               # TF-IDF vectorizer
├── tfidf_matrix.pkl        # TF-IDF feature matrix
│
├── requirements.txt        # Python dependencies
├── .env.example            # Environment variable template
├── .gitignore              # Git ignored files
└── README.md               # Project documentation
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/priyankpancholi11/movie-recommendation-system.git
```

### 2. Navigate to the Project Directory

```bash
cd movie-recommendation-system
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it:

**Windows:**
```bash
.venv\Scripts\activate
```

**Linux / macOS:**
```bash
source .venv/bin/activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure TMDB API Key

Create a `.env` file in the project root directory.

Add your TMDB API key:

```env
TMDB_API_KEY=your_tmdb_api_key_here
```

Replace the placeholder with your actual TMDB API key.

### 6. Run the Backend

Open a terminal and execute:

```bash
uvicorn main:app --reload
```

The FastAPI backend will run at:

`http://127.0.0.1:8000`

API documentation:

`http://127.0.0.1:8000/docs`

### 7. Run the Frontend

Open another terminal, activate the virtual environment, and execute:

```bash
streamlit run app.py
```

The Streamlit application will open in your browser.

## 🔑 API Integration

This project uses the TMDB API to retrieve movie information and related data.

You need your own TMDB API key to access the external movie data.

## 📌 Future Improvements

- Improve recommendation accuracy.
- Explore deep learning-based recommendation techniques.
- Add user-based personalized recommendations.
- Improve search and filtering capabilities.
- Deploy the application online.

## 👨‍💻 Author

**Priyank Pancholi**

B.Tech – Information Technology (2023–2027)

GitHub: [@priyankpancholi11](https://github.com/priyankpancholi11)

---

*Developed as a Machine Learning project to explore content-based recommendation systems and API-based application development.*
