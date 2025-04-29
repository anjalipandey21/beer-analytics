# 🍺 Craft Beer Recommender System Using Crowdsourced Reviews

## 📘 Project Overview
This project builds a personalized, content-based recommender system for craft beers using crowdsourced reviews. The system takes user-preferred product attributes (e.g., "fruity", "bold", "crisp") and recommends beers by analyzing real user reviews. The solution leverages NLP, cosine similarity, sentiment analysis, and both Bag-of-Words and word embedding approaches to deliver tailored recommendations.

---

## 🧠 What This Project Does
- Scrapes and cleans beer reviews from publicly available sources (~2,000+ reviews).
- Extracts top product attributes using text frequency and co-occurrence analysis.
- Computes similarity between user preferences and reviews using Bag-of-Words.
- Performs sentiment analysis on each review using VADER.
- Scores beers using a combination of similarity and sentiment.
- Recommends top 3 beers tailored to user-specified attributes.
- Compares recommendations generated via Bag-of-Words vs. Word Embeddings.
- Explores alternate recommendation strategies based on average ratings.
- Finds the most similar beer to a selected one among a chosen subset.

---

## 📊 Key Features & Insights
- Combines **semantic similarity** and **sentiment polarity** for better recommendations.
- Attributes such as *malty*, *fruity*, *robust*, etc., are extracted from actual data, not predefined lists.
- Uses **lift ratio analysis** to ensure co-occurrence strength between selected attributes.
- Demonstrates how **word embeddings (spaCy)** can influence recommendation diversity.
- Provides a comparative analysis between **ratings-only** and **attribute-driven** approaches.

---

## ⚙️ Technologies Used
- `Python 3.x`
- `BeautifulSoup`, `Requests` (data scraping)
- `NLTK`, `VADER`, `spaCy` (NLP & sentiment)
- `Scikit-learn` (cosine similarity, vectorization)
- `Pandas`, `NumPy` (data wrangling)
- `Matplotlib`, `Seaborn` (visualization)
- `Jupyter Notebook` (development & documentation)

---

## 📂 Project Structure
- `Assignment_2_Unstructured.ipynb`: Main notebook with data collection, analysis, modeling, and visualizations.
- `README.md`: Project summary and documentation.

---

## 🚀 How to Run
1. Clone the repository and open the Jupyter notebook.
2. Ensure required libraries are installed:
   ```bash
   pip install beautifulsoup4 requests nltk vaderSentiment spacy scikit-learn pandas matplotlib seaborn
   python -m spacy download en_core_web_md
