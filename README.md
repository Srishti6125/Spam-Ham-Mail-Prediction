# 🎶 Song Recommendation System  

## 🚀 Problem Statement  
With the ever-growing volume of music across streaming platforms, users often struggle to discover new tracks that match their taste. Traditional recommendation systems either rely on metadata (artist, genre) or popularity, which can miss the personal and lyrical context behind songs.  

This project builds a **hybrid recommendation system** that combines **musical features** and **lyrical content** to suggest songs similar to a given input.  

---

## 🧩 Approach  
1. **Dataset**: Collected song metadata, audio features, and lyrics.  
2. **Preprocessing**:  
   - Cleaned text (stopword removal, lemmatization).  
   - Converted duration & loudness to numeric.  
   - Handled missing values.  
3. **Feature Engineering**:  
   - **Textual features** → TF-IDF on lyrics, genre, album.  
   - **Numerical features** → Tempo, Loudness, Energy, Danceability, Positiveness, etc. (scaled with MinMax).  
   - Combined into a single hybrid feature matrix.  
4. **Similarity Calculation**: Used **Cosine Similarity** on the combined matrix.  
5. **Fuzzy Matching**: Handled spelling errors/typos in user queries.  
6. **Recommendation Output**: Pretty-printed top-N recommended songs with artists.  

---

## 📌 Summary  
The system recommends songs that are **both musically and lyrically relevant** to the input track. It leverages a **hybrid content-based filtering** approach instead of relying solely on popularity or metadata.  

---

## ✅ Results & Conclusion  
- Successfully recommends songs with better **diversity** and **relevance** compared to basic content-based models.  
- Handles user input variation (misspellings, case differences).  
- Demonstrates scalability for large music datasets.  

---

## 🔮 Future Scope  
- Add **collaborative filtering** for personalized user-based recommendations.  
- Integrate **Word2Vec, LSTM, or Transformer models** for deeper lyric understanding.  
- Deploy as a **web app (Streamlit/Flask)** with real-time recommendations.  
- Include **audio signal processing features** (MFCC, Chroma, Spectral contrast).  

---
