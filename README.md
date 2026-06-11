# 🎬 CineMatch - Movie Recommendation System

A full-stack Movie Recommendation System built using **Python, FastAPI, Streamlit, Docker, and AWS EC2**.

The application helps users discover movies through intelligent recommendations powered by **TF-IDF content-based filtering** and real-time movie data from **TMDB (The Movie Database)**.

---

## 🚀 Live Demo

**Live Application:**
http://3.26.201.177:8501

---

## 📌 Features

### 🎥 Movie Search

* Search movies using TMDB API
* Autocomplete movie suggestions
* View movie posters and details

### 🤖 Recommendation Engine

* Content-based recommendation system
* TF-IDF vectorization on movie metadata
* Similar movie recommendations based on movie descriptions

### 🎭 Genre Recommendations

* Additional recommendations based on movie genres
* Real-time TMDB integration

### 📄 Movie Details Page

* Movie overview
* Release date
* Genres
* Poster and backdrop images

### ☁️ Cloud Deployment

* Dockerized application
* Hosted on AWS EC2
* Publicly accessible web application

---

# 🏗️ Project Architecture

```text
User
 │
 ▼
Streamlit Frontend
 │
 ▼
FastAPI Backend
 │
 ├── TF-IDF Recommendation Engine
 │
 └── TMDB API Integration
```

---

# 🛠️ Tech Stack

### Frontend

* Streamlit

### Backend

* FastAPI
* Uvicorn

### Machine Learning

* Scikit-Learn
* TF-IDF Vectorizer
* Cosine Similarity

### Data Processing

* Pandas
* NumPy

### Deployment

* Docker
* Docker Hub
* AWS EC2

### External API

* TMDB API

---

# 📂 Project Structure

```text
movies/
│
├── app.py                 # Streamlit Frontend
├── main.py                # FastAPI Backend
│
├── df.pkl                 # Movie dataset
├── tfidf.pkl              # TF-IDF vectorizer
├── tfidf_matrix.pkl       # TF-IDF matrix
├── indices.pkl            # Movie indices
│
├── Dockerfile
├── requirements.txt
├── .env
│
└── movies_metadata.csv
```

---

# ⚙️ Installation

## Clone Repository

```bash
git clone https://github.com/shreyashagrawal00/movies_recommendation.git

cd movies_recommendation
```

---

## Create Virtual Environment

```bash
python -m venv venv
```

Activate:

### Windows

```bash
venv\Scripts\activate
```

### Linux / Mac

```bash
source venv/bin/activate
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Configure Environment Variables

Create a `.env` file:

```env
TMDB_API_KEY=your_tmdb_api_key
```

---

## Run FastAPI Backend

```bash
uvicorn main:app --reload
```

---

## Run Streamlit Frontend

```bash
streamlit run app.py
```

---

# 🐳 Docker Deployment

Build Docker Image:

```bash
docker build -t movie-rec-app .
```

Run Container:

```bash
docker run -p 8501:8501 movie-rec-app
```

---

# ☁️ AWS Deployment

The application is deployed using:

* AWS EC2
* Docker
* Docker Hub

Deployment workflow:

```text
VS Code
   ↓
Docker Build
   ↓
Docker Hub
   ↓
AWS EC2
   ↓
Public Application
```

---

# 📊 Machine Learning Approach

The recommendation engine uses:

### TF-IDF Vectorization

Converts movie descriptions into numerical vectors.

### Cosine Similarity

Measures similarity between movies.

Workflow:

```text
Movie Description
       ↓
TF-IDF Vectorizer
       ↓
Feature Matrix
       ↓
Cosine Similarity
       ↓
Recommended Movies
```

---

# 📈 Future Improvements

* User authentication
* Collaborative filtering
* Hybrid recommendation system
* Movie watchlist
* User ratings and reviews
* Dark/Light mode
* Advanced filtering options

---

# 👨‍💻 Author

**Shreyash Agrawal**

* GitHub: https://github.com/shreyashagrawal00
* LinkedIn: [www.linkedin.com/in/shreyashagrawal00](http://www.linkedin.com/in/shreyashagrawal00)

---

# ⭐ If you like this project

Give it a star on GitHub and feel free to contribute.
