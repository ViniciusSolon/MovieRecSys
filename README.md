# MovieRecSys 🎬  
A **content-based** movie recommendation system using **cosine similarity** for similarity measurement.

## 📌 Features
- Extracts key metadata (genres, cast, keywords, and overview).
- Processes textual data with **stemming** and feature extraction using `CountVectorizer`.
- Computes **cosine similarity** to find the closest movies.
- Returns the **top 5 most similar** movies based on the given title.

## 🚀 Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ViniciusSolon/MovieRecSys.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure the dataset files (`dataset_filmes.csv` and `dataset_elenco.csv`) are in the root directory.

## 🛠 How to Use
Run the script and call:
```python
recommend_movie('The Avengers')
```
Example output:
```
Iron Man
Captain America: The First Avenger
Thor
The Incredible Hulk
Guardians of the Galaxy
```

## 📂 Dataset
The system uses structured datasets:
- `dataset_filmes.csv`: Movie details such as title, overview, genres, and keywords.
- `dataset_elenco.csv`: Cast and crew details.

## 🔍 How It Works
1. **Data Preprocessing:**  
   - Cleans and extracts relevant information.
   - Applies **stemming** to process textual data.
   - Creates **tags** by combining relevant metadata.

2. **Feature Extraction & Similarity Calculation:**  
   - Converts tags into vectors using `CountVectorizer`.
   - Computes **cosine similarity**, which measures similarity between movies.

3. **Recommendation System:**  
   - Finds movies with the highest similarity to the given title.
   - Returns the **top 5 most similar** movies.

## 📌 Dependencies
- `numpy`
- `pandas`
- `scikit-learn`
- `nltk`

## 📜 License
This project is licensed under the **MIT License**.

## 🤝 Contributing
Suggestions and improvements are welcome! Feel free to submit a PR or open an issue.

---
Developed with ❤️ by **Vinicius Solon Cordeiro**
