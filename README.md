# 🎶 Song Recommendation System  

## 📌 Overview  
Music streaming platforms provide millions of tracks, but finding the *right* song can often feel overwhelming. This project implements a **content-based song recommendation system** that suggests songs similar to a given input based on both:  

- **Textual features** → Lyrics, artist, genre, album, emotions  
- **Audio features** → Tempo, loudness, danceability, energy, acousticness, etc.  

By combining text and numeric data into a **hybrid feature matrix**, the system generates meaningful, context-aware recommendations.  

---

## 🚀 Features  
✅ Hybrid recommendation using both text and audio features  
✅ Fuzzy matching to handle typos in user input  
✅ Cosine similarity for measuring song similarity  
✅ Tabular output of Top-N recommended songs  
✅ Scalable and extendable for larger datasets  

---

## ⚙️ Tech Stack  
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, NLTK, Tabulate, Matplotlib, Seaborn  
- **Techniques:**  
  - TF-IDF Vectorization (lyrics & text features)  
  - MinMax Scaling (numerical audio features)  
  - Cosine Similarity (recommendation engine)  

---

## 📂 Dataset & Source  
The dataset used contains song metadata, lyrics, and acoustic properties such as:  
- 🎵 **Song Metadata:** Title, Artist(s), Album, Genre, Emotion  
- 🎼 **Text Features:** Lyrics (cleaned & preprocessed)  
- 🎚 **Audio Features:** Tempo, Energy, Loudness, Danceability, Acousticness  

**Source:** [Kaggle - Spotify/Custom Dataset] *(replace with your dataset link if public)*  

---

## 📑 Project Workflow  
1. **Data Preprocessing**  
   - Converted audio length & loudness to numerical format  
   - Handled missing values in lyrics and numeric columns  
   - Preprocessed lyrics: lowercasing, punctuation removal, stopwords removal, lemmatization  

2. **Feature Engineering**  
   - TF-IDF vectorization for lyrics & text metadata  
   - MinMaxScaler for audio features  
   - Concatenation of textual + numerical features  

3. **Recommendation Engine**  
   - Cosine similarity to compute closeness between songs  
   - Fuzzy matching to allow flexible input (e.g., handling typos)  
   - Tabular output showing recommended songs and artists  

---

## 🎵 Example Usage  

```python
# Example input
Enter song name: Shivers

# Example output (Top-5 Recommendations)

╒══════════════════════════╤════════════════════════╕
│ Song                     │ Artist(s)              │
╞══════════════════════════╪════════════════════════╡
│ Shiver Shiver            │ WALK THE MOON          │
│ Shivers                  │ Haris                  │
│ Shivers                  │ Rachel Platten         │
│ Shivers Remix            │ Ed Sheeran,Jessi,SUNMI │
│ Sleep with the lights on │ The Wanton Bishops     │
╘══════════════════════════╧════════════════════════╛

---

## ✅ Results & Conclusion  

The hybrid recommendation system successfully suggests songs that are both **musically** and **lyrically** similar to the input. Compared to basic content-based filtering, this hybrid approach:  

- 🎯 Improves recommendation quality  
- 🎶 Provides diversity in suggested tracks  
- ✍️ Handles spelling errors and user input variation  

---

## 🔮 Future Scope  

- 👥 Add **collaborative filtering** for user-based personalization  
- 🧠 Integrate **Word2Vec / LSTM / Transformer models** for deeper lyric understanding  
- 🌐 Deploy as an interactive **web app (Streamlit/Flask)**  

---
