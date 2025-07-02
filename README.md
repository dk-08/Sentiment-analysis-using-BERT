# Sentiment Analysis on Trustpilot Reviews using BERT

This project uses a pretrained BERT model to perform sentiment analysis on real customer reviews scraped from [Trustpilot](https://www.trustpilot.com/review/meesho.com). It classifies each review on a **1–5 star scale**, providing insight into customer satisfaction and feedback quality.

---

## 🚀 Features

* ✅ Scrapes reviews from Trustpilot (e.g., Meesho.com)
* ✅ Uses `nlptown/bert-base-multilingual-uncased-sentiment` model
* ✅ Classifies sentiment from 1 (very negative) to 5 (very positive) stars
* ✅ Handles multilingual and informal text
* ✅ Outputs results to a Pandas DataFrame for further analysis

---

## 📦 Dependencies

Install required libraries with:

```bash
pip install transformers torch pandas beautifulsoup4 requests
```

> You may also need `selenium` if scraping JavaScript-heavy pages.

---

## 📂 Project Structure

```text
.
├── file.ipynb                  # Jupyter Notebook with full workflow
├── README.md                   # Project description
└── requirements.txt            # Python dependencies
```

---

## 🧪 How It Works

1. **Scrape reviews** from Trustpilot using `requests` + `BeautifulSoup`.
2. **Clean and tokenize** text using Hugging Face's tokenizer.
3. **Run predictions** through a pretrained BERT model.
4. **Map logits** to sentiment labels (1–5 stars).
5. **Visualize or export** sentiment scores for analysis.

---

## 📊 Sample Output

```text
Review: "The product was decent but arrived late."
Predicted: 3★ (Neutral)
```

---

## 📘 Model Info

* **Model**: [`nlptown/bert-base-multilingual-uncased-sentiment`](https://huggingface.co/nlptown/bert-base-multilingual-uncased-sentiment)
* **Classes**: 1–5 stars
* **Languages**: Multilingual (100+ supported)

---

## ✅ Use Cases

* E-commerce product review analysis
* Brand perception tracking
* Feedback classification and tagging
* Customer support prioritization

---

## 📄 License

This project is for educational and research use only. Check each website's [Terms of Service](https://legal.trustpilot.com/) before scraping or using their data.

---
Feel free to fork and contribute :))


