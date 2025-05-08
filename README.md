# Personalized Job Matching using NLP

This project implements a resume-based job recommendation system using Natural Language Processing (NLP). It compares two text similarity methods—TF-IDF and MiniLM (a transformer-based embedding model)—to match resumes with job descriptions.

## 📁 Structure

- `notebooks/`: Contains the main Jupyter notebooks for preprocessing, embedding, and evaluation.
- `data/`: JSON job listings and sample resumes.
- `scripts/`: Utility scripts (e.g., data loading, preprocessing).
- `results/`: Charts and visualizations generated for the report.

## 🧠 Methods

- **TF-IDF**: Frequency-based keyword matching using scikit-learn.
- **MiniLM**: Semantic similarity using sentence-transformers (`all-MiniLM-L6-v2`).
- **Seniority Filtering**: Regex-based job level classification (intern, new_grad, mid, senior, executive).

## 📝 Evaluation

Participants ranked job matches based on perceived relevance to their resume (1 = most relevant, 10 = least relevant). MiniLM outperformed TF-IDF in most cases, especially for senior-level resumes.

## 🚀 Requirements

- Python 3.8+
- `scikit-learn`
- `pandas`
- `spacy`
- `sentence-transformers`
- `matplotlib`, `seaborn`
- `PyMuPDF` (for PDF resume parsing)
