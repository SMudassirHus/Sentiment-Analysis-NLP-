# Alexa Sentiment (Streamlit)

Sentiment analysis of Amazon Alexa reviews.  
Model = **TF-IDF (1–2 grams)** + **Logistic Regression** (handles phrases like “don’t like”, “not good”).

**Live demo:** https://huggingface.co/spaces/Mudassir110/alexa-sentiment
**Made by Mudassir**

---

## What’s inside
- `streamlit_app.py` – UI for single text & CSV bulk prediction
- `Models/`
  - `countVectorizer.pkl` – TfidfVectorizer (1–2 grams)
  - `scaler.pkl` – identity transformer (kept for compatibility)
  - `model_xgb.pkl` – LogisticRegression (filename kept for app code)
- `requirements.txt` – deps to run the app

## Run locally
```bash
pip install -r requirements.txt
streamlit run streamlit_app.py
