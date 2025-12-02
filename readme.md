## Project Overview

This project explores how languages can be represented and compared using character-level trigram frequencies. Each language is converted into a high-dimensional vector based on how often each trigram appears in its text corpus. These vectors are used to measure similarity between languages and to visualize their relationships using UMAP, revealing clear clusters that align with known language families.

A lightweight neural classifier (a small MLP) is trained on the same trigram features to identify the language of new text samples. The model achieves strong performance, with a weighted F1 score of around 0.95, showing that simple statistical features can capture meaningful orthographic patterns.

Overall, the project demonstrates how compact representations derived from raw text can be used for language comparison, visualization, and classification, all without requiring deep linguistic knowledge or complex models.

## Purpose of the Project

1. **Build trigram-based language representations**  
   Each language is converted into a normalized vector of trigram frequencies, capturing its orthographic structure.

2. **Measure similarity between languages**  
   Cosine distance is used to create a similarity matrix that highlights expected relationships, especially within Romance and Germanic families.

3. **Visualize language structure**  
   UMAP projects the high-dimensional vectors into 2D, revealing clear clusters and cross-language patterns.

4. **Train a simple neural classifier**  
   A small MLP (Linear → ReLU → Linear) learns to identify the language of short text samples using the trigram features.

5. **Evaluate model performance**  
   Accuracy, precision, recall, and F1 score show that the classifier generalizes well, even with a shallow architecture.

6. **Lay the groundwork for interactive tools**  
   The methods developed here support future visual or exploratory applications for comparing languages.
