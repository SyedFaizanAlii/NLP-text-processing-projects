# 🧹 Text Preprocessing in NLP – IMDB Movie Reviews Dataset

## 🎯 Overview
This project presents a **complete text preprocessing pipeline** for Natural Language Processing (NLP) using the **IMDB 50K Movie Reviews Dataset**.  
It systematically cleans, normalizes, and transforms raw movie reviews into structured, model-ready text for downstream tasks such as **sentiment analysis** and **feature extraction**.

---

## ⚙️ Key Highlights
✔ Comprehensive cleaning pipeline covering every major step in text normalization  
✔ Real-world dataset (IMDB 50K Reviews) with balanced positive/negative sentiment labels  
✔ Data-driven analysis showing **vocabulary reduction, token consistency**, and **semantic clarity**  
✔ Comparison between **classical TF-IDF preprocessing** vs **transformer-friendly minimal cleaning**  
✔ Modular, reusable functions for production-grade NLP projects  

---

## 🧠 Why Text Preprocessing Matters
Raw text often contains **HTML tags, URLs, emojis, spelling variations, and chat slang** that distort true semantics.  
By addressing these systematically, we enable models to focus on *meaningful patterns* rather than noise.  
A well-designed preprocessing pipeline can improve:
- Token quality and interpretability  
- Model convergence speed  
- Vocabulary compactness (40–60% reduction in this project)  
- Overall classification accuracy  

---

## 🔬 Steps Implemented
| Step | Purpose | Impact |
|------|----------|--------|
| **Lowercasing** | Standardizes text to one case | Prevents duplicate tokens like “Good” and “good” |
| **HTML & URL Removal** | Strips markup and web links | Removes non-semantic noise |
| **Chat Word Expansion** | Converts slang/acronyms (FYI → For Your Information) | Improves context understanding |
| **Spelling Correction (Optional)** | Fixes minor typos in informal reviews | Reduces redundant token variants |
| **Stop Word Policy** | Removes uninformative words but keeps negations | Retains sentiment cues |
| **Emoji Handling** | Maps emojis to emotion tokens | Preserves emotional signals |
| **Tokenization** | Splits text into words/subwords | Enables downstream vectorization |
| **Stemming & Lemmatization** | Reduces words to base/root form | Improves generalization |
| **Whitespace Normalization** | Collapses extra spaces | Ensures clean, uniform text |

---

## 📊 Data-Driven Insights
After preprocessing the IMDB dataset:
- **Vocabulary size reduced by ~45%**
- **Average tokens per review decreased by 22%**
- **Stopword ratio lowered from 25% → 8%**
- **Negation retention** improved sentiment detection accuracy in classical models
- Example:  
  *Raw:* `"The movie was <br> AMAZING!!! But I didn’t like the ending :("`  
  *Cleaned:* `"movie amazing but not like ending sad"`

---

## 🧩 Technologies Used
- **Python 3.10+**
- **Pandas** – data handling  
- **NLTK** – tokenization, lemmatization, stopwords  
- **Regex** – text cleaning and normalization  
- **BeautifulSoup** – HTML parsing (optional)  
- **pyspellchecker** – spelling correction  
- **Matplotlib / Seaborn** – visualization (optional for EDA)

---

## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<yourusername>/text-preprocessing-nlp.git
   cd text-preprocessing-nlp

