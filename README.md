# Tweet Sentiment Analysis using Naive Bayes

This project performs **sentiment classification** on Twitter data using a **Multinomial Naive Bayes** classifier. It leverages **NLTK** for preprocessing and **scikit-learn** for modeling, transforming tweets into numerical vectors using **CountVectorizer**.

---

## Dataset

The dataset includes labeled tweets for training and testing:

- `train_Pos.en` — Positive training tweets  
- `train_Neg.en` — Negative training tweets  
- `ttestPos.en` — Positive testing tweets  
- `ttestNeg.en` — Negative testing tweets  

 **Download the dataset from Google Drive**:  
🔗 [Click here to access the dataset folder](https://drive.google.com/drive/folders/142_nDPZZnr-g7Mdq0uy8s-VZvQF-O1Bz?usp=share_link)

## 📌 Key Features

✅ Clean and preprocess tweet text (lowercasing, tokenization, stopword removal, lemmatization)  
✅ Convert tweets into numerical features using `CountVectorizer`  
✅ Train a Naive Bayes classifier for sentiment prediction  
✅ Real-time user input for tweet classification  
✅ Accuracy score printed after testing on unseen data  
✅ Modular, easy-to-read Python code structure

---

## Model Workflow

```mermaid
flowchart TD
    A[Load Dataset] --> B[Preprocess Text]
    B --> C[Tokenize & Lemmatize]
    C --> D[CountVectorizer]
    D --> E[Train MultinomialNB]
    E --> F[Predict on Test Data]
    F --> G[Print Accuracy]
    E --> H[Predict on User Input]
