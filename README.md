# 🎬 Movie Search Engine – Information Retrieval Project

A search & ranking engine built on the TMDB 5000 Movies dataset, comparing multiple Information Retrieval approaches.

## What it does
- Cleans and preprocesses movie metadata (title, overview, cast, director, genres, languages)
- Builds an **Inverted Index** over titles and overviews
- Builds a **TF-IDF + Cosine Similarity** search model with weighted fields (title, overview, cast, director)
- Implements **BM25** ranking (`rank_bm25`) for query-based retrieval
- Evaluates retrieval quality using **Precision@K** on a set of test queries (e.g. "brad pitt", "batman", "spider man")

## Tech Stack
- Python, Pandas
- Scikit-learn (TF-IDF, cosine similarity)
- rank-bm25
- ast (parsing stringified JSON columns from the dataset)

## Files
- `movie_search_ir.ipynb` — full notebook: data cleaning → indexing → TF-IDF model → BM25 model → evaluation

## Dataset
TMDB 5000 Movies & Credits dataset (not included in this repo — download from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) .
