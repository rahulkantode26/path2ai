# NLP Basics & NLP Models

Assignments covering the fundamentals of text preprocessing and two core ways to turn text into numbers: TF-IDF and Word2Vec.

## Contents

| File | Description |
|------|-------------|
| `nlp_basics_assignments.ipynb` | Jupyter notebook with all 3 assignments, code, and explanations |
| `NLP_Basics_Summary.pdf` | 1-2 page written summary of key learnings |
| `README.md` | This file |

## Assignments

**1. Text Cleaning & Tokenization**
Cleaned 25 movie reviews via lowercasing, punctuation removal, tokenization (NLTK), and stopword removal.

**2. TF-IDF Implementation**
Converted the cleaned reviews into TF-IDF vectors using `sklearn.TfidfVectorizer`; explored feature names, matrix shape, and top words per document.

**3. Word2Vec Embeddings**
Trained a `gensim` Word2Vec model on the same dataset to find similar words and inspect word vectors; compared TF-IDF vs Word2Vec.

## How to Run

1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install nltk gensim scikit-learn pandas numpy
   ```
3. Open the notebook:
   ```bash
   jupyter notebook nlp_basics_assignments.ipynb
   ```
4. Run all cells (first run will download small NLTK data packages: `punkt`, `stopwords`).

## Dataset

A small hand-written set of 25 movie reviews (mix of positive and negative sentiment), defined directly in the notebook — no external dataset file needed.

## Key Takeaways

- Text must be cleaned and tokenized before it can be turned into numbers.
- TF-IDF is fast, interpretable, and frequency-based — good for search/ranking, works fine on small datasets.
- Word2Vec captures word meaning and context via dense vectors, but needs much more data to be reliable.
