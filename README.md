 ## Book Recommendation System

This project implements a content-based book recommendation system that recommends books based on writing style and semantic similarity, rather than user ratings, reviews, or interaction data.
The project is developed using Natural Language Processing (NLP) techniques and transformer-based sentence embeddings.

## Project Overview

Traditional recommendation systems rely heavily on user behavior. This project addresses the **cold-start problem** by recommending books using only textual information such as:
- Book title
- Author
- Publisher
The system compares books based on semantic similarity of writing style.

## Technologies Used

- Python  
- Pandas, NumPy  
- Sentence Transformers (`all-MiniLM-L6-v2`)  
- Scikit-learn (Cosine Similarity)  
- Jupyter Notebook
- 
## Approach

1. Load and clean book metadata from a public CSV dataset  
2. Preprocess text by normalizing and removing noise  
3. Generate sentence embeddings using a pretrained transformer model  
4. Compute cosine similarity between all book embeddings  
5. Recommend top-N books with similar writing styles  
6. Filter out books by the same primary author to ensure diversity  

## Evaluation

- Metric used:Cosine similarity (qualitative)
- Strengths: Fast inference, scalable, no user data required
- Limitations:Limited text representation and no personalization

## Ethical Considerations

- No personal or user data is used
- Recommendations may reflect biases present in the dataset
- The system is intended for educational and demonstration purposes


