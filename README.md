
# 📺 Anime Recommendation System

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)

An intuitive and feature-rich anime recommendation system built using Python and machine learning. It uses various models like Cosine Similarity, K-Nearest Neighbors, Random Forest, and Naive Bayes for generating personalized anime suggestions based on the synopsis content. The system also features a user-friendly graphical interface developed with `tkinter`.

![GUI Screenshot](https://i.imgur.com/YOUR_SCREENSHOT.png)

## 🧠 Features

- 📚 **Multiple ML Models**: Cosine Similarity (Count & TF-IDF), KNN, Random Forest, and Naive Bayes.
- ✨ **Content-Based Filtering**: Recommends anime based on synopsis similarity.
- 🖥️ **Graphical User Interface**: Simple and sleek GUI for user interaction using `tkinter`.
- 🎨 **Anime Wallpaper Background**: Enhanced UI experience with themed background.
- 📝 **Flexible Input**: Search for recommendations by entering any anime title.

## 🗂️ Project Structure

```
Anime-Recommendation-System/
│
├── anime_list.csv                  # Dataset containing anime titles, synopses, and scores
├── anime_recommender.ipynb        # Main Jupyter Notebook with ML and GUI code
├── README.md                       # Project documentation
```

## 🔧 Tech Stack

- **Languages**: Python
- **Libraries**:
  - `pandas`, `numpy`, `scikit-learn` — Data processing and ML
  - `tkinter`, `PIL` — GUI design
  - `requests`, `io` — Image fetching and display
- **Models Used**:
  - CountVectorizer / TfidfVectorizer + Cosine Similarity
  - K-Nearest Neighbors (KNN)
  - Random Forest Regressor
  - Naive Bayes Classifier

## 🏗️ How It Works

1. **Data Loading & Preprocessing**: Removes duplicates and null synopses.
2. **Feature Extraction**: Converts synopsis text into vector format using CountVectorizer and TfidfVectorizer.
3. **Model Training**:
   - **Cosine Similarity**: For content-based recommendations.
   - **KNN**: Identifies the closest animes in synopsis space.
   - **Random Forest**: Predicts anime scores based on content features.
   - **Naive Bayes**: Learns likelihood of title categories based on synopsis.
4. **GUI**:
   - Enter anime title.
   - Select model from dropdown.
   - View top 10 recommendations in a scrollable output area.

## 🚀 How to Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/Anime-Recommendation-System.git
   cd Anime-Recommendation-System
   ```

2. **Install dependencies**:
   ```bash
   pip install pandas numpy scikit-learn pillow requests
   ```

3. **Run the script**:
   - Use the Jupyter notebook: `anime_recommender.ipynb`
   - Or run the GUI directly by copying the code into a `.py` file and executing it:
     ```bash
     python anime_recommender.py
     ```

## 🧪 Example Usage

- Input: `Naruto`
- Model: `Cosine Similarity with TfidfVectorizer`
- Output:
  ```
  1. Bleach
  2. One Piece
  3. Fairy Tail
  ...
  ```

## 📊 Models Comparison

| Model                               | Type             | Strengths                             |
|------------------------------------|------------------|----------------------------------------|
| Cosine Similarity (Count/TF-IDF)   | Content-Based    | Simple, fast, and interpretable        |
| K-Nearest Neighbors (KNN)          | Memory-Based     | Good for finding closely related items |
| Random Forest Regressor            | Ensemble         | Captures nonlinear patterns            |
| Naive Bayes                        | Probabilistic    | Lightweight and fast                   |

## 📌 Notes

- The recommendation system is entirely **content-based**, relying only on anime synopses.
- Ensure that `anime_list.csv` includes the following columns: `title`, `synopsis`, `score`.

## 💡 Future Improvements

- Add hybrid filtering combining content and user ratings
- Deploy as a web app using Flask or Streamlit
- Include more metadata (e.g., genres, release year) for improved accuracy

## 👤 Author

**Your Name**  
[GitHub](https://github.com/yourusername) • [LinkedIn](https://www.linkedin.com/in/yourprofile)

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
