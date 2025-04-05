# System-Development-for-Marketing-
# Recommender Systems with Collaborative Filtering and SVD++

## Overview

This project implements and compares two types of recommender systems:
- **Collaborative Filtering (User-based KNN)**
- **SVD++ (Matrix Factorization with Implicit Feedback)**

The models are evaluated on two datasets: **MovieLens 100k** and a **Netflix Prize sample**.  
The goal is to predict user ratings accurately and recommend **new, diverse, and novel** movies.

Evaluation focuses on:
- Hit Rate
- Novelty
- Diversity
- RMSE (Root Mean Squared Error)

---

## Project Structure

| File | Description |
|:---|:---|
| `Collaborative Filtering User Based KNN.ipynb` | User-based collaborative filtering using cosine similarity, average rating adjustment, and hybrid approaches. |
| `SVD++ Movielens.ipynb` | SVD++ model training and evaluation on the Movielens dataset. |
| `SVD++ Netflix.ipynb` | SVD++ model training and evaluation on the Netflix dataset. |
| `Netflix EDA.ipynb` | Exploratory Data Analysis (EDA) for the Netflix dataset. |
| `Movielens EDA.ipynb` | Exploratory Data Analysis (EDA) for the Movielens dataset. |
| `movie_titles.csv` | Netflix movie titles metadata. |
| `movies.dat` | Movielens movie metadata file. |
| `ratings.dat` | Movielens user-item ratings data. |
| `users.dat` | Movielens user demographic information. |
| `power point persentation.pptx` | Presentation summarizing methodology, evaluation, and results. |


---

## Models Implemented

- **Collaborative Filtering (UserKNN)**:
  - Standard cosine similarity
  - UserKNN with average rating adjustment
  - Hybrid UserKNN (combining rating patterns and average behavior)
  - User classification based on rating profiles
  
- **SVD++ (Matrix Factorization)**:
  - Incorporates both explicit ratings and implicit feedback
  - Trained with Stochastic Gradient Descent (SGD)
  - Based on the logic and structure proposed in Koren (2008)

---

## Evaluation Metrics

- **Hit Rate**: Measures if recommended items were unseen by the user.
- **Novelty**: Encourages recommendations of less popular, more unique items.
- **Diversity**: Ensures recommended items are different from each other.
- **RMSE**: Measures prediction error between predicted and true ratings.

---

## References

- **Paper**: Factorization Meets the Neighborhood: A Multifaceted Collaborative Filtering Model  
- **Author**: Yehuda Koren  
- **Published In**: Proceedings of the 14th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, 2008  
- **Link**: [https://dl.acm.org/doi/10.1145/1401890.1401944](https://dl.acm.org/doi/10.1145/1401890.1401944)

**Citation (APA Format):**  
Koren, Y. (2008). Factorization meets the neighborhood: A multifaceted collaborative filtering model. *Proceedings of the 14th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, 426–434. [https://doi.org/10.1145/1401890.1401944](https://doi.org/10.1145/1401890.1401944)

---

## Results and Outcomes

- Both Collaborative Filtering and SVD++ achieved low RMSE scores, with around 1 star prediction error.
- **SVD++** achieved:
  - Better diversity (more varied movie recommendations)
  - Higher novelty (less mainstream movie suggestions)
  - Slightly improved RMSE compared to CF
- The systems successfully recommended **new**, **diverse**, and **novel** movies to users, enhancing discovery and engagement.

---


