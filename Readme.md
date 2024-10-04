<h1 align="center">🎬 Movie Recommendation System 🎬</h1>

<p align="center">
  A machine learning-based recommendation system that suggests movies similar to your favorite ones! 🔍✨
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue" />
  <img src="https://img.shields.io/badge/Scikit--learn-0.24-orange" />
  <img src="https://img.shields.io/badge/Pandas-1.3.3-yellowgreen" />
  <img src="https://img.shields.io/badge/NumPy-1.21-lightblue" />
  <!-- <img src="https://img.shields.io/github/license/basharul2002/Movie-Recommendation-System" /> -->
</p>

---

## 📖 Overview

This **Movie Recommendation System** suggests similar movies based on user input by analyzing movie data, including genres, keywords, cast, director, and tagline. The system uses **TF-IDF Vectorization** and **Cosine Similarity** to calculate similarity scores and recommend movies accordingly.

## 💡 Features
- **Input Matching**: Finds the closest match to the movie name you input
- **Movie Recommendations**: Suggests up to 30 similar movies based on textual features (e.g., genre, cast, director)
- **Efficient NLP Processing**: Leverages **TF-IDF Vectorization** for efficient text comparison and recommendation generation

## 🛠️ Technologies Used

- **Python**: The core programming language used for the implementation
- **NumPy**: Used for numerical computations
- **Pandas**: For handling and manipulating the dataset
- **Scikit-learn**: To implement **TF-IDF Vectorization** and calculate **Cosine Similarity**
- **Difflib**: For finding close matches of movie names in the dataset

## 🗂 Dataset
- The dataset is stored in a CSV file named `movies_dataset.csv`
- **Relevant features used**:
  - `Genres`
  - `Keywords`
  - `Tagline`
  - `Cast`
  - `Director`

---

## 🚀 How It Works

1. **Data Preprocessing**: Combines the selected features (`genres`, `keywords`, `tagline`, `cast`, and `director`) into a single string for each movie, filling in missing values with empty strings.
   
2. **Vectorization**: Converts the combined text data into **TF-IDF vectors** to transform the textual information into numerical features.

3. **Cosine Similarity Calculation**: Computes the **Cosine Similarity** between the input movie and every other movie in the dataset to determine how similar they are.

4. **Movie Recommendations**: Based on similarity scores, the system suggests movies that are most similar to the one provided by the user.

---

## ⚙️ How to Run

Follow these steps to run the system locally:

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/basharul2002/Movie-Recommendation-System.git
```

### 2️⃣ Install Dependencies
Make sure you have the necessary libraries installed. Run the following command:
```bash
pip install numpy pandas scikit-learn
```

### 3️⃣ Run the Python Script
Ensure the dataset is in the correct path (e.g., `sample/movies_dataset.csv`), and then execute the script:
```bash
python movie_recommendation_system.py
```

### 4️⃣ Enter Your Favorite Movie
When prompted, input the movie name:
```bash
Enter your favourite movie name: Iron Man
```

## 📊 Example Output

```bash
Movies suggested for you:

1. Iron Man
2. Iron Man 2
3. Iron Man 3
4. Avengers: Age of Ultron
5. The Avengers
6. Captain America: Civil War
7. Captain America: The Winter Soldier
8. Ant-Man
9. X-Men
10. Made
11. X-Men: Apocalypse
12. X2
13. The Incredible Hulk
14. The Helix... Loaded
15. X-Men: First Class
16. X-Men: Days of Future Past
17. Captain America: The First Avenger
18. Kick-Ass 2
19. Guardians of the Galaxy
20. Deadpool
21. Thor: The Dark World
22. G-Force
23. X-Men: The Last Stand
...
26. The Last Airbender
27. Southland Tales
28. Zathura: A Space Adventure
29. Sky Captain and the World of Tomorrow
```


## 📂 Directory Structure

```
Movie-Recommendation-System/
│
├── sample/
│   └── movies_dataset.csv   # The movie dataset
├── movie_recommendation.py  # Main Python script
└── README.md                # Documentation
```

<!--
---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).
