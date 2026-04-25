# 🎬 Movie Recommender System

A content-based movie recommender system built with **Python** and **Streamlit** that suggests similar movies based on your selection, complete with movie posters fetched from TMDB API.

🚀 **Live Demo:** [movie-recommender-system-i7xaeuth9qlsvncbwk37k4.streamlit.app](https://movie-recommender-system-i7xaeuth9qlsvncbwk37k4.streamlit.app)

---

## 📸 Screenshot

![Movie Recommender System](https://image.tmdb.org/t/p/w500/jRXYjXNq0Cs2TcJjLkki24MLp7u.jpg)

---

## ✨ Features

- 🔍 Search or select any movie from the dropdown
- 🎯 Get **5 similar movie recommendations** instantly
- 🖼️ Displays **movie posters** fetched live from TMDB API
- ⚡ Fast and lightweight Streamlit interface
- ☁️ Fully deployed on Streamlit Cloud

---

## 🛠️ Tech Stack

| Technology | Usage |
|---|---|
| Python | Core programming language |
| Streamlit | Web application framework |
| Scikit-learn | Cosine similarity model |
| Pandas | Data manipulation |
| Pickle | Model serialization |
| TMDB API | Fetching movie posters |
| Google Drive | Hosting large model files |
| GitHub | Version control & deployment |

---

## 📁 Project Structure

```
movie-recommender-system/
│
├── model/
│   ├── movie_list.pkl       # Movie dataset (loaded from Google Drive)
│   └── similarity.pkl       # Similarity matrix (loaded from Google Drive)
│
├── app.py                   # Main Streamlit application
├── requirements.txt         # Python dependencies
├── .gitignore               # Ignores pkl files and venv
└── README.md                # Project documentation
```

---

## ⚙️ How It Works

1. The model uses a **content-based filtering** approach
2. Movie metadata is vectorized and cosine similarity is computed
3. When a user selects a movie, the top 5 most similar movies are returned
4. Movie posters are fetched in real-time using the **TMDB API**

---

## 🚀 Run Locally

### 1. Clone the repository
```bash
git clone https://github.com/soumojitbasu/movie-recommender-system.git
cd movie-recommender-system
```

### 2. Create a virtual environment
```bash
python -m venv .venv
.venv\Scripts\activate      # Windows
source .venv/bin/activate   # Mac/Linux
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the app
```bash
streamlit run app.py
```

---

## 📦 Requirements

```
streamlit
requests
scikit-learn
pandas
numpy
gdown
```

---

## 🌐 Deployment

This app is deployed on **Streamlit Cloud**.

- Model files (`movie_list.pkl`, `similarity.pkl`) are stored on **Google Drive**
- Downloaded automatically at runtime using `gdown`
- No large files stored in the GitHub repository

---

## 🔑 API Key

This project uses the [TMDB API](https://www.themoviedb.org/documentation/api) to fetch movie posters.

---

## 👨‍💻 Author

**Soumojit Basu**
- GitHub: [@soumojitbasu](https://github.com/soumojitbasu)

---

## ⭐ Show Your Support

If you found this project helpful, please give it a **star** on GitHub! ⭐
