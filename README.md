# 📊 Amazon Product Review Sentiment Dashboard

This project analyzes customer sentiment from **Amazon product reviews** and presents it visually using interactive charts. The goal is to help understand how customers feel about different products over time using natural language processing and data visualization techniques.

---

## 📌 Project Highlights

- 🧹 **Clean and process** real Amazon review data
- 🧠 **Assign sentiment labels** (positive, neutral, negative) based on review ratings
- 🕵️‍♂️ **Combine title + text** for improved sentiment analysis
- 📈 **Visualize sentiment distribution and trends** over time using Plotly
- 🔍 Easy to extend with classification models or dashboards

---

## 🗂️ Dataset Description

The dataset contains Amazon product reviews and includes columns like:

- `reviews.title` — Title of the review
- `reviews.text` — Review content
- `reviews.rating` — Rating (1 to 5)
- `reviews.date` — Date when the review was written
- `sentiment` — Derived label (positive, neutral, negative)

---


---

## ⚙️ Requirements

Install the dependencies with:

```bash
pip install -r requirements.txt


Key Libraries:

pandas for data manipulation

plotly for interactive charts

nltk, regex for text processing

scikit-learn for future model support



🚀 How It Works
Load and clean data:

Combine reviews.text and reviews.title into one column

Create a sentiment column from reviews.rating:

rating >= 4 → positive

rating == 3 → neutral

rating <= 2 → negative

Visualize using Plotly:

📊 Sentiment Distribution Pie Chart

📈 Sentiment Trend Line Chart (based on reviews.date)

📊 Bar Chart of Sentiment Counts

(Optional): Use BERT tokenizer + LSTM for sentiment prediction.

📊 Dashboard Visuals
1. Sentiment Distribution
An interactive pie chart showing the percentage of positive, neutral, and negative reviews.

2. Sentiment Trend Over Time
Line chart of sentiment counts grouped by week or month — useful for spotting trends in public opinion.

3. Bar Chart
Shows absolute number of reviews per sentiment category.


🧠 Future Enhancements
🔍 Add a BERT + LSTM sentiment classifier

🧵 Word clouds or keyword extraction for each sentiment

🌐 Deploy using Streamlit or Dash

📩 Export insights to CSV or PDF

⚖️ Handle class imbalance (SMOTE or class weights)




