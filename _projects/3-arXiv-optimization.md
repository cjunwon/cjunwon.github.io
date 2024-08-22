---
title: "Research  Paper Classification Optimization Using NLP and Instance-Based Learning"
excerpt: "Mathematics 156 - Machine Learning (UCLA)<br/><br/><img src='/images/arxiv_optimization.png' style='box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.3);'>"
collection: projects
---

### About

This project aims to develop efficient classification for research papers using Natural Language Processing (NLP) and Instance-Based Learning. This project was developed for the [Mathematics 156 - Machine Learning](https://catalog.registrar.ucla.edu/course/2022/math156?siteYear=2022) course at UCLA.

### Background & Motivation

The arXiv is a free distribution service and an open-access archive for scholarly articles in the fields of physics, mathematics, computer science, quantitative biology, quantitative finance, and statistics. The arXiv is a valuable resource for researchers to share their work and stay up-to-date with the latest research in their field. While the current site provides various search and filtering options, including a map that visualizes the connections between papers based on citations, there is no built-in classification system that groups papers by topic.

This project aims to develop an efficient classification system for research papers based on its abstract. The goal is to provide a tool that quickly identifies existing papers related to their research topic of interest, allowing for a layer of prevention in overlap and redundancy in research.

### Methodology & Key Concepts

1. **Data Collection**
   - The dataset used for this project is the [arXiv dataset](https://www.kaggle.com/Cornell-University/arxiv) from Kaggle.
   - The dataset contains metadata for over 1.7 million papers from the arXiv.
   - The metadata includes the paper ID, title, abstract, authors, categories, and publication date.
       - In the context of this project, only the abstract and categories are used.

2. **Data Preprocessing**
    - The abstracts are preprocessed using NLP techniques.
    - The abstracts are tokenized, lemmatized, and vectorized using the TF-IDF vectorizer.
    - The categories are one-hot encoded.
    - The dataset is split into training and testing sets.

3. **Instance-Based Learning**

    We test several techniques for instance-based learning:

    - After TF-IDF vectorization:
        - Truncated Singular Value Decomposition (SVD) --> Density-Based Spatial Clustering of Applications with Noise (DBSCAN)
        - K-Means Clustering (K-Means++) --> Approximate Nearest Neighbors (ANNOY)
        - K-Nearest Neighbors (KNN)
        - Random Forest
    - Directly using FastText embeddings

### Relevant Files

The following slides were used as part of the final project presentation.

[Download  PDF](/files/MATH156_presentation.pdf)
<iframe src="/files/MATH156_presentation.pdf" width="100%" height="500"></iframe>

---

The following report provides a detailed overview of the project.

[Download  PDF](/files/MATH156_report.pdf)
<iframe src="/files/MATH156_report.pdf" width="100%" height="850"></iframe>