# Predicting Emotional States in Twitter Using NLP & Embeddings

This project uses NLP and embedding models to classify tweets by emotion (normal, stressed, lonely, anxious) and explore how emotional expression clusters topically.

We trained and compared multiple modeling approaches, then applied the best-performing model to 20,000+ unlabeled tweets and analyzed emotional and gender patterns across semantic clusters.

---

## Data Sources

Two Kaggle datasets:
- **Behavioral Tweets** (emotion-labeled)
- **Twitter User Gender Classification**

Combined total: ~40,000 tweets.

---

## Approach

1. Sampled tweets to avoid memory limits in R.
2. Repeated training 50 times to reduce sampling bias.
3. Benchmarked three approaches:
   - GloVe embeddings + k-means
   - TF-IDF + k-means
   - GloVe embeddings + Random Forest (best model)
4. Applied sentence-transformer embeddings (BERT) for clustering and visualization on 20k new tweets.

---

## Models & Tools

- **R:** text2vec, ranger, tidyverse
- **Python:** sentence-transformers, scikit-learn
- **Techniques:** TF-IDF, GloVe, Random Forest, k-means, UMAP, BERT embeddings

---

## Key Results

- Random Forest + embeddings achieved the highest accuracy.
- BERT embeddings formed **10 meaningful semantic clusters**.
- Certain clusters concentrated stressed/anxious tweets.
- Gender patterns emerged across clusters (brands vs. male vs. female).

These findings align with research on mental health expression online.

---

## Project Highlights

- Repeated sampling + model averaging  
- Cross-language workflow (R + Python)  
- Topic clustering using embeddings  
- Emotional + gender distribution analysis  


