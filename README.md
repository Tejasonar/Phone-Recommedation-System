Phone Recommendation System

A Content-Based Recommendation System that suggests smartphones to users based on their preferences such as price, processor, RAM, storage, camera,
battery capacity, and Android version.
The system uses TF-IDF Vectorization and Cosine Similarity to compare user requirements with available phones and recommend the closest matches.

---

Project Objective

Build a smart recommendation engine for smartphones.
Allow users to enter their requirements and get relevant suggestions.
Apply feature extraction & similarity algorithms to rank phones.
Provide accurate and personalized recommendations.

---

Dataset Description

The dataset includes detailed smartphone specifications:

Brand & Model
Price
Processor (Snapdragon, MediaTek, Dimensity, etc.)
RAM & Storage
Battery Capacity
Rear & Front Camera
Android Version
Additional features

---

Data Preprocessing

Removed duplicate phones
Cleaned inconsistent units (GB, mAh, MP)
Handled missing values
Standardized all text (lowercase, spacing, formatting)
Merged specifications into a single combined feature column

---

Feature Engineering

Cleaned text (remove special characters, stopwords)
TF-IDF Vectorization applied on combined text features
Created vectors for:
Phone specifications
User input/query
Calculated similarity scores using Cosine Similarity

---

Recommendation Process

User enters preferences (price, RAM, processor, etc.)
Input is converted into a TF-IDF feature vector
Similarity is calculated between user input and all phones
Phones are ranked based on similarity score
Top N phones are returned as recommendations

---

Algorithms Used
TF-IDF Vectorizer (sklearn)
Cosine Similarity (distance measure)
Optional: Weighted scoring (price importance, RAM priority, etc.)

---

Evaluation

Since this is a content-based recommender system, evaluation is done through:
Relevance of recommended phones
Similarity scores
Manual validation based on specifications
No ML accuracy/precision metrics are used.

---   

Key Features

Personalized phone suggestions
Multi-parameter filtering
Fast and lightweight
Fully content-based (no user ratings needed)
Easy to integrate with UI (Streamlit/Flask)
