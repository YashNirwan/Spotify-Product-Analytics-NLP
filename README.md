# Spotify-Product-Analytics-NLP
Mining 20,000 real user reviews to prioritize the product roadmap and reduce churn. Tech Stack: Python, NLTK, VADER, Pandas.

# 🎧 Voice of Customer Analysis: Spotify Product Strategy

**Role:** Product Analyst / Strategist
**Tools:** Python (Pandas, NLTK), VADER Sentiment Analysis, Seaborn
**Dataset:** 20,000 Real Spotify App Reviews (Kaggle)

## 📌 Executive Summary
User feedback is high-volume and unstructured. This project automates the analysis of **20,000 user reviews** to identify the root causes of churn. By applying NLP (Sentiment Analysis), I moved beyond anecdotal evidence to quantify specific friction points in the user journey.

## 📊 Key Insights (The "Aha" Moment)
My analysis revealed that **17% of total reviews were negative**, significantly impacting the NPS score.

### 1. The "Shuffle" Friction
* **Finding:** The keyword **"Random"** appeared in **319** negative reviews.
* **User Pain Point:** Users feel the shuffle algorithm is repetitive, playing the same songs despite large libraries.
* **Strategic Recommendation:** Prioritize a **"True Random" Toggle** feature in the next sprint (Low Effort / High Impact).

### 2. The "Update" Regression
* **Finding:** A spike in negative sentiment correlated with the word **"Update"** (357 mentions).
* **User Pain Point:** Recent UI changes caused playlist management to crash on Android devices.
* **Strategic Recommendation:** Halt rollout of v8.4 to Android users and initiate a QA investigation into memory leaks.

## 🛠️ Technical Approach
1.  **Ingestion:** Loaded raw CSV data and filtered for the most recent 20,000 reviews to ensure relevance.
2.  **Processing:** Cleaned text data (removed stopwords like "app", "music") to isolate descriptive adjectives.
3.  **Sentiment Scoring:** Used **VADER (Valence Aware Dictionary and sEntiment Reasoner)** to assign polarity scores (-1 to +1) to every review.
4.  **Visualization:** Built Word Clouds and Sentiment Distribution charts to communicate findings to stakeholders.

## 📈 Visual Artifacts
*(Note: Upload your images here to show recruiters what you built)*

## 🚀 How to Run This Code
1.  Clone the repository.
2.  Install dependencies: `pip install pandas nltk wordcloud matplotlib`
3.  Run `Spotify_Sentiment_Analysis.ipynb` in Jupyter or Google Colab.
