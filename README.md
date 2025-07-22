# 🎬 Movie Data Analysis – Netflix Style

This project performs a comprehensive exploratory data analysis (EDA) on a Netflix-style movie dataset from Kaggle, focusing on genres, popularity, voting behavior, and movie release trends. The goal is to derive meaningful insights about movie trends and audience preferences.

---

## 📦 Dataset

- **Source**: [MyMovieDB Dataset](https://www.kaggle.com/datasets/parikhsamir/mymoviedb)
- **Total Records**: 9,827 rows × 9 columns
- **Features Included**:
  - `Title`: Movie title
  - `Release_Date`: Release year of the movie
  - `Genre`: Genre(s) of the movie (comma-separated)
  - `Popularity`: Popularity score
  - `Vote_Average`: Average user votes
  - `Overview`, `Original_Language`, `Poster_Url`: Dropped during cleaning for analysis relevance

---

## 🧼 Data Cleaning & Preprocessing

1. **Checked for duplicates and null values**  
   ➤ Result: No NaNs or duplicate rows

2. **Dropped irrelevant columns**  
   ➤ Dropped `Overview`, `Original_Language`, and `Poster_Url`

3. **Date conversion**  
   ➤ Converted `Release_Date` into year format only

4. **Vote_Average categorization**  
   ➤ Created 4 categories:
   - `not_popular`
   - `below_avg`
   - `average`
   - `popular`

5. **Genre preprocessing**  
   ➤ Split comma-separated genres into lists  
   ➤ Exploded rows so each movie-genre pair gets its own row  
   ➤ Converted to `category` data type

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 Most Frequent Genre
- **Drama** is the most frequent genre.
- Appears in over 14% of all genre occurrences.

<img width="511" height="500" alt="genre3" src="https://github.com/user-attachments/assets/98dbaaf4-8b90-4d1b-8e33-91afcae689fd" />

---

### 🔹 Vote_Average Distribution
- 25.5% of movies fall into the `popular` category.
- Drama again leads as the top genre in terms of popularity.

<img width="511" height="500" alt="votes" src="https://github.com/user-attachments/assets/03eed404-1a79-4d0a-bbfa-64869cc14777" />

---

### 🔹 Movie with Highest Popularity
- **Title**: *Spider-Man: No Way Home*
- **Genres**: Action, Adventure, Sci-Fi

<img width="801" height="159" alt="Screenshot 2025-07-22 104849" src="https://github.com/user-attachments/assets/d02272b7-6949-4acb-b5a4-1a03485fbf25" />

---

### 🔹 Movie with Lowest Popularity
- **Title**: *The United States, Thread*
- **Genres**: Music, Drama, War, Sci-Fi, History

<img width="891" height="273" alt="Screenshot 2025-07-22 105113" src="https://github.com/user-attachments/assets/9643f7cf-d5a4-457e-9642-fa9bed960ad6" />

---

### 🔹 Most Active Release Year
- **Year**: **2020**
- Contains the highest number of movie releases.

<img width="640" height="480" alt="film" src="https://github.com/user-attachments/assets/1d007e5b-d069-4b86-971b-99e23c840a57" />

---

## 🧠 Key Insights

> ### Q1: What is the most frequent genre in the dataset?
**Drama** is the most common genre, appearing in more than 14% of records.

> ### Q2: Which genre has the highest votes?
Again, **Drama** leads with 18.5% of the `popular` vote category.

> ### Q3: Which movie got the highest popularity score?
*Spider-man: No Way Home* with multiple genres including Action, Sci-Fi, and Adventure.

> ### Q4: Which movie got the lowest popularity score?
*The United States, Thread* with multiple genres including Drama, Sci-Fi, and War.

> ### Q5: Which year has the most filmed movies?
**2020** holds the record for the most movies released in the dataset.

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 📁 Project Structure

