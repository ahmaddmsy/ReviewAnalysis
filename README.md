# Shopee Review Sentiment Analysis with IndoBERT

🚀 **Sentiment Analysis on Shopee Product Reviews using IndoBERT**

## 📌 Overview
This project analyzes sentiment from Shopee product reviews using **Natural Language Processing (NLP)** techniques. The pipeline includes **text preprocessing, normalization, stopword removal, stemming**, and **sentiment classification using IndoBERT**. The final processed data is saved in **Parquet** and **Feather** formats for efficient storage and analysis.

## 🔥 Features
✅ **Efficient Data Processing**: Uses Modin (Dask) for scalable Pandas operations.  
✅ **Advanced Text Cleaning**: Handles emojis, punctuation, stopwords, and spelling corrections.  
✅ **IndoBERT Sentiment Analysis**: Utilizes pre-trained **IndoBERT-Lite-Base** for sentiment classification.  
✅ **Batch Processing Optimization**: Processes data in batches for improved performance on large datasets.  
✅ **Optimized Storage**: Saves results in **Parquet** and **Feather** for fast I/O operations.  

## 📂 Dataset
- Source: **Shopee product reviews**
- File: `DatasetShopee.csv`
- Fields: `username`, `rating`, `comment`, `comment_clean`, `sentimen_bert`

## 🛠️ Tech Stack
- **Python 3.11.9**
- **Modin (Dask backend)** – Faster Pandas
- **SymSpell** – Spell correction
- **Sastrawi** – Stemming & stopword removal
- **Transformers (Hugging Face)** – IndoBERT sentiment analysis
- **Torch (PyTorch)** – GPU acceleration

## 🏗️ Installation & Setup
### 1️⃣ Clone Repository
```bash
 git clone https://github.com/yourusername/shopee-review-analysis.git
 cd shopee-review-analysis
```

### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Run Sentiment Analysis
```bash
python preprocess_and_sentiment.py
```

## 📊 Output Files
- `DatasetShopee_Bersih.parquet` → Optimized storage format
- `DatasetShopee_Bersih.feather` → Fast I/O operations

## 📌 Example Preprocessed Data
| Username  | Rating | Comment (Raw) | Comment Clean | Sentimen BERT |
|-----------|--------|--------------|---------------|---------------|
| user_123  | 5      | Mantaaaap! | mantap | Positive |
| user_456  | 3      | Lumayan sih, tp lama | lumayan lama | Neutral |
| user_789  | 1      | Gacoooor! barang rusak | gacor barang rusak | Negative |

## 🔗 References
- IndoBERT Model: [Hugging Face Model](https://huggingface.co/indobenchmark/indobert-lite-base-p1)
- Shopee Reviews Dataset (Private)

## 🤝 Contributing
Contributions are welcome! Feel free to open an issue or submit a pull request.

## 📜 License
This project is licensed under the **MIT License**.

---
📢 **Let's connect!** If you have any feedback or questions, feel free to reach out on [LinkedIn](https://linkedin.com/in/yourprofile).

