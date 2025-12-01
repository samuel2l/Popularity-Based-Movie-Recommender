# Popularity-Based Recommendation System

This project implements a **popularity-based recommendation system** using two datasets: `ratings.csv` and `movies.csv`. The system recommends movies based on their overall popularity — calculated from the number of ratings and average rating — rather than individual user preferences.

---

## What is a Popularity-Based Recommender?

A popularity-based recommendation system suggests items that are widely liked or frequently consumed by all users. In this case, the most-rated and highest-rated movies are recommended to everyone.

This approach is:
- Simple and fast  
- Useful when user history is unavailable (cold start problem)  
- Ideal for a homepage or trending section  

---

## Datasets Used

### 1. `ratings.csv`  
Contains user ratings for movies

**Columns:**
- `userId`  
- `movieId`  
- `rating`  
- `timestamp`  

Download:  
https://drive.google.com/file/d/12yJB_ivy-8TMUBtRF_PXQd_dIikpoQ52/view  

---

### 2. `movies.csv`  
Contains movie information

**Columns:**
- `movieId`  
- `title`  
- `genres`  

Download:  
https://drive.google.com/file/d/1_ed-D9jaIFUimurItNV1nSmb39sBxZ4s/view  

---

## How the System Works

1. Load both datasets (`ratings.csv` and `movies.csv`)  
2. Group ratings by `movieId`  
3. Calculate:  
   - Average rating  
   - Number of ratings  
4. Sort movies by:  
   - Highest average rating  
   - Highest number of ratings  
5. Merge results with `movies.csv` to get movie titles  
6. Display top N popular movies  

The output is a list of the most popular movies based on real user ratings.

---

## Tech Stack

- Python  
- Pandas  
- Jupyter Notebook / VS Code  

---

## Features

- No user login required  
- Handles large datasets  
- Fast performance  
- Great solution for a “Trending Movies” section  

---

## How To Use

1. Download the datasets from the links above  
2. Place them in the same folder as your `main.py` or Jupyter Notebook  
3. Run the script  
4. Get top popular movie recommendations  

---
> Based on the tutorial from Data Mentor.  
> Video: https://www.youtube.com/watch?v=kPxASj5wJBY&list=PLZLuc8eJafeGM6VF3kijsJZBJ9CspQy7x  
