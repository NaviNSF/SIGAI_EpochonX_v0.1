# PROJECT PREDICTION USING DISCORD BOT

### OVERVIEW:

This project provides a recommendation system that suggests relevant AI and technology-related projects based on a student's current project. The recommendation system leverages a clustering algorithm (DBSCAN) to group projects based on their names and technologies used. Using TF-IDF vectorization and cosine similarity, the system finds and recommends the most relevant projects from the same cluster.

### FUNCTIONS:

We used different things like:-
- Clustering Algorithm (DBSCAN): Groups projects into clusters based on their description and technology stack.
- TF-IDF Vectorization: Converts text data (project names and technologies used) into numerical vectors for comparison.
- Cosine Similarity: Measures the similarity between the user's current project and the projects in the dataset.

### How does it work?

1. Data Preprocessing:

-  The project names and technologies are concatenated to create a corpus of project descriptions.

2.TF-IDF Vectorization:

  - The corpus is converted into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) to represent the importance of terms in each project description.

3.Clustering:

  - The DBSCAN algorithm is used to cluster the projects based on their descriptions. Projects within the same cluster are considered related.

4.Project Recommendation:

  - A user inputs their current project description.

  - The system calculates the cosine similarity between the user's input and all projects in the dataset.
  
  - It finds the most similar project and recommends other projects from the same cluster, sorted by their similarity score.

   
