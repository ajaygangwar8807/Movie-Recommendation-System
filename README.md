🎬 Movie Recommendation System

A real-world End-to-End Machine Learning project that recommends movies based on content similarity using Natural Language Processing (NLP), TF-IDF Vectorization, and Cosine Similarity.

The system provides intelligent movie recommendations by analyzing movie metadata and finding similar movies based on their textual features. The project is deployed with a Streamlit user interface and powered by a FastAPI backend.

---

🚀 Project Overview

Recommendation systems are widely used by platforms such as Netflix, Amazon Prime Video, Disney+, and Spotify to improve user experience through personalized suggestions.

This project demonstrates how to build a Content-Based Movie Recommendation System from scratch and deploy it using modern Python technologies.

---

✨ Features

✅ Content-Based Movie Recommendation

✅ Natural Language Processing (NLP)

✅ TF-IDF Vectorization

✅ Cosine Similarity Matching

✅ FastAPI Backend

✅ Streamlit Interactive UI

✅ Real-Time Recommendations

✅ Pickle-Based Model Serialization

✅ Production-Ready Architecture

---

🛠️ Tech Stack

Machine Learning & NLP

- Python
- Pandas
- NumPy
- Scikit-Learn
- NLTK

Backend

- FastAPI
- Uvicorn

Frontend

- Streamlit

Data Storage

- CSV Dataset
- Pickle Files (.pkl)

---

📂 Project Structure

MOVIE-RECOMMENED/
│
├── app.py                 # Streamlit UI
├── main.py                # FastAPI Backend
│
├── movies_metadata.csv    # Movie Dataset
│
├── df.pkl                 # Processed Movie Data
├── indices.pkl            # Movie Index Mapping
├── tfidf.pkl              # Trained TF-IDF Vectorizer
├── tfidf_matrix.pkl       # TF-IDF Feature Matrix
│
├── requirements.txt       # Project Dependencies
├── .env                   # Environment Variables
├── .gitignore             # Ignored Files
│
├── .venv/
└── __pycache__/

---

🔄 Project Workflow

1. Data Collection

The movie dataset contains:

- Movie Titles
- Genres
- Keywords
- Cast Information
- Crew Information
- Movie Overview

---

2. Data Cleaning

The dataset is cleaned by:

- Removing duplicates
- Handling missing values
- Dropping irrelevant columns
- Standardizing textual features

---

3. NLP Text Preprocessing

Text data is preprocessed using:

- Lowercasing
- Tokenization
- Stopword Removal
- Stemming
- Text Normalization

This improves the quality of feature extraction.

---

4. Feature Engineering

Important movie attributes are combined into a single textual representation.

Example:

Action Adventure Space Alien Future War

This acts as a movie profile for similarity comparison.

---

5. TF-IDF Vectorization

TF-IDF (Term Frequency – Inverse Document Frequency) converts text into numerical vectors.

Benefits:

- Captures important words
- Reduces the impact of common words
- Creates meaningful numerical representations

---

6. Cosine Similarity

Cosine Similarity measures how similar two movies are.

A higher score indicates greater similarity between movies.

The recommendation engine ranks movies based on these similarity scores.

---

7. Recommendation Engine

When a user selects a movie:

1. The movie is searched in the dataset.
2. Its vector representation is retrieved.
3. Similarity scores are calculated.
4. Movies are ranked.
5. Top recommendations are returned.

---

8. Model Serialization

To avoid retraining every time:

- df.pkl
- indices.pkl
- tfidf.pkl
- tfidf_matrix.pkl

are stored and loaded directly during inference.

---

9. FastAPI Backend

FastAPI is used to:

- Handle recommendation requests
- Process movie queries
- Return recommendation results
- Provide API endpoints

Benefits:

- High Performance
- Automatic Documentation
- Easy Integration

---

10. Streamlit Frontend

Streamlit provides:

- User-Friendly Interface
- Interactive Search Experience
- Real-Time Recommendation Display

Users simply enter a movie name and receive recommended movies instantly.

---

⚙️ Installation

Clone Repository

git clone https://github.com/your-username/movie-recommendation-system.git

Navigate to Project Folder

cd movie-recommendation-system

Create Virtual Environment

python -m venv .venv

Activate Virtual Environment

Windows

.venv\Scripts\activate

Linux / Mac

source .venv/bin/activate

Install Dependencies

pip install -r requirements.txt

---

▶️ Run Streamlit Application

streamlit run app.py

Application will start at:

http://localhost:8501

---

▶️ Run FastAPI Backend

uvicorn main:app --reload

Backend will start at:

http://127.0.0.1:8000

---

📖 API Documentation

FastAPI automatically generates Swagger documentation.

Visit:

http://127.0.0.1:8000/docs

to test API endpoints directly from your browser.

---

🎯 Learning Outcomes

This project helps understand:

- Recommendation Systems
- Natural Language Processing
- TF-IDF Vectorization
- Cosine Similarity
- Feature Engineering
- FastAPI Development
- Streamlit Development
- Machine Learning Deployment
- API Design and Integration

---

🚀 Future Improvements

- TMDB API Integration
- Movie Posters and Ratings
- User Authentication
- Personalized Recommendations
- Hybrid Recommendation System
- Docker Support
- AWS / Render / Railway Deployment

---

🤝 Contributing

Contributions, issues, and feature requests are welcome.

Feel free to fork the repository and submit a pull request.

---

⭐ Support

If you found this project useful, please consider giving it a star on GitHub.

---

📜 License

This project is created for educational and learning purposes.

---

Made with ❤️ using Python, NLP, FastAPI, Streamlit, and Machine Learning.