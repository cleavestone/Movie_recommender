# Movie_recommender
## MOVIE RECOMMENDATION
### Project Introduction

The aim of this project is to build a content-based movie recommender system that suggests movies similar to a given movie. By leveraging movie metadata such as genres, cast, crew, and keywords, the system provides personalized movie recommendations.

### Project Outline
**Data Collection and Preprocessing**

1. Datasets: Utilized Movies metadata, Keywords, and Credits datasets.
2. Merging: Combined datasets on the 'id' column.
3. Cleaning: Cleaned the 'id' column, dropped duplicates, and handled missing values.
4.Feature Selection: Selected relevant columns: title, overview, genres, cast, crew, keywords.

**Data Cleaning and Normalization**
1. Text Normalization: Converted text data to lowercase.
2. Genres Conversion: Transformed genres into a list of genre names.
3. Feature Combination: Combined genres and overview into a single text feature.
   
**Word2Vec Model Training**
1. Tokenization: Tokenized the combined features of each movie.
2. Model Training: Trained a Word2Vec model on the tokenized corpus to learn word embeddings. Feature Extraction

**Description Vectors: Computed the average Word2Vec vector for each movie's description. Similarity Computation**

Cosine Similarity: Calculated cosine similarity between movie embeddings to identify similar movies.
Recommendation Function

Top Recommendations: Created a function to fetch the top 10 most similar movie recommendations for a given movie.
