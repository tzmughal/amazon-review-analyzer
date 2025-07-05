# 📦 Amazon Product Review Analyzer

Perform sentiment analysis on Amazon product reviews using **TextBlob** and visualize key insights to identify top positive and negative customer concerns.

---

## 🚀 Overview

This project analyzes Amazon product reviews using **NLP** techniques to:
- Determine the overall sentiment (positive, negative)
- Generate word clouds of frequently used positive and negative terms
- Highlight common issues or praised features based on customer feedback

---

## 🧠 Technologies Used

- **TextBlob** – For sentiment polarity and subjectivity analysis
- **Pandas** – For data manipulation and preprocessing
- **Seaborn** & **Matplotlib** – For data visualization
- **WordCloud** – To generate visual clouds of sentiment-rich keywords

---

## 📊 Sample Visualizations

(images/1.png)

(images/2.png)

---

#### 📌 Sample Code Snippet

```python
from textblob import TextBlob

def analyze_sentiment(review):
    analysis = TextBlob(review)
    polarity = analysis.sentiment.polarity
    if polarity > 0:
        return 'Positive'
    elif polarity < 0:
        return 'Negative'
    else:
        return 'Neutral'

