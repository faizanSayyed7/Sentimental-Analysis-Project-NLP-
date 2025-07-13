## Amazon Fine Food Reviews Sentiment Analysis 🍽️

This repository contains a Jupyter notebook that performs **sentiment analysis** on Amazon Fine Food Reviews. The goal is to classify customer reviews as positive, negative, or neutral, providing insights into customer satisfaction. We leverage two powerful sentiment analysis algorithms: **VADER** (Valence Aware Dictionary and sEntiment Reasoner) and **RoBERTa** (A Robustly Optimized BERT Pretraining Approach), and then compare their performance.

---

### What's Inside? 📂

The core of this project is a detailed Jupyter notebook (`notebook528e79bced.ipynb`) that walks you through the entire sentiment analysis pipeline.

**Here's what you'll find:**

* **Data Loading and Exploration**: We begin by loading the `Reviews.csv` dataset, which contains a vast collection of Amazon food reviews. Initial **Exploratory Data Analysis (EDA)** is performed to understand the distribution of review scores and the nature of the textual data.
    * The dataset is sourced from Amazon Fine Food Reviews.
    * A quick look at the data reveals columns such as `Id`, `ProductId`, `UserId`, `ProfileName`, `HelpfulnessNumerator`, `HelpfulnessDenominator`, `Score`, `Time`, `Summary`, and `Text`.
    * The `Text` column, which contains the actual review content, is the primary focus for sentiment analysis.
    * An initial EDA step involves visualizing the count of reviews by star ratings, providing a quick overview of customer sentiment.
    * For efficiency, the notebook initially processes a subset of 5000 reviews from the full dataset.

---

### The Algorithms 🤖

We explore two distinct approaches to sentiment analysis:

#### 1. VADER (Valence Aware Dictionary and sEntiment Reasoner)

**VADER** is a lexicon and rule-based sentiment analysis tool specifically attuned to sentiments expressed in social media. It is effective because it considers:

* **Lexicon**: A dictionary of words with sentiment scores.
* **Rules**: It accounts for punctuation, capitalization, degree modifiers (e.g., "very good"), and conjunctions that can alter sentiment.

In this project, VADER is used to assign a sentiment score to each review, categorizing them as positive, negative, or neutral based on its compound score.

#### 2. RoBERTa (A Robustly Optimized BERT Pretraining Approach)

**RoBERTa** is a transformer-based language model, an optimized version of BERT. It’s known for its strong performance in various natural language processing (NLP) tasks, including sentiment analysis. Unlike VADER, which is rule-based, RoBERTa understands sentiment by processing the context and nuances of language through its extensive pre-training on large text corpora.

In this notebook, RoBERTa is fine-tuned or directly used for sentiment prediction on the Amazon reviews, leveraging its deep understanding of language to capture complex sentiment expressions.

---

### Comparison of VADER and RoBERTa ⚖️

A crucial part of this project is the **comparison of VADER and RoBERTa's performance**. The notebook provides insights into:

* **Accuracy**: How well each algorithm predicts the actual sentiment of the reviews.
* **Strengths and Weaknesses**: VADER is typically faster and works well for general sentiment, while RoBERTa, being a deep learning model, can capture more complex and subtle sentiments but requires more computational resources.
* **Use Cases**: Understanding when to use one over the other based on the specific requirements of a sentiment analysis task.

By analyzing the results, you'll gain a comprehensive understanding of each algorithm's effectiveness in the context of food review sentiment.

---

### How to Use 🚀

1.  **Clone the Repository**:
    `git clone <repository_url>`
2.  **Navigate to the Directory**:
    `cd <repository_name>`
3.  **Open the Jupyter Notebook**:
    `jupyter notebook notebook528e79bced.ipynb`
