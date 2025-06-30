# Hotel Review Sentiment Analyzer

This project analyzes hotel customer reviews to classify sentiment and extract service-related insights such as "room service", "food quality", or "staff friendliness". It is built entirely in Google Colab using Python, with no external AI platforms required.

# Objective

- Classify hotel reviews into Positive or Negative sentiment.
- Extract top service-related topics mentioned by customers.
- Summarize customer satisfaction and identify key strengths or pain points.
- Generate a structured CSV report for analysis and business insights.


# Tools & Libraries Used

- Google Colab
- Python 3
- Transformers pipeline for sentiment analysis
- KeyBERT for topic extraction
- Pandas & Matplotlib for data handling and visualization
- Kaggle for dataset

# Dataset

**Source**: [515K Hotel Reviews Data in Europe – Kaggle](https://www.kaggle.com/datasets/jiashenliu/515k-hotel-reviews-data-in-europe)
- Merged `Negative_Review` and `Positive_Review` into a single `review` column.
- Cleaned text by removing punctuation, lowercasing, and removing stopwords.

# Features
[1] Sentiment Analysis
Uses Hugging Face’s transformer models to classify sentiment for each review.
[2] Topic Extraction
Extracts top 5 keywords/service areas using KeyBERT to identify:
- Room service
- Cleanliness
- Food quality
- Staff friendliness
- Amenities, etc.

# Visual Insights
- Bar chart of sentiment distribution
- Horizontal bar chart of most mentioned service topics

# Export
- Final output CSV: `hotel_review_sentiment_output.csv`
- Includes columns: `review`, `clean_review`, `sentiment`, `topics`

