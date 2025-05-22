# 🧠 BART-Based Abstractive Text Summarization for News Articles

## 📌 Business Objective

Text summarization condenses long content into shorter, meaningful versions. This project leverages the **BART (Bidirectional and Auto-Regressive Transformer)** model to perform **abstractive summarization**, which allows the model to generate summaries in its own words, rather than copying exact sentences from the original.

### 💼 Applications
- Scientific Research  
- Financial Reports  
- Legal Documentation  
- Literature Reviews  
- Meeting Summaries  
- Programming Documentation  

## 📊 Dataset Overview

The dataset consists of **40,000 professionally written summaries** of news articles in CSV format with the following columns:

- **Title** – Headline of the article  
- **Summary** – Human-written summary  
- **URL** – Link to the original article  
- **Date** – Publication date  
- **Content** – Full article text  

## 🎯 Project Aim

To apply and fine-tune the **BART model** for generating abstractive summaries of news articles using a deep learning approach.

## 🛠️ Tech Stack

- **Programming Language:** Python  
- **Key Libraries:**  
  - `pandas` for data handling  
  - `scikit-learn` for preprocessing  
  - `transformers` (Hugging Face) for model and tokenizer  
  - `torch` (PyTorch) for deep learning  
- **Environment:** Google Colab (GPU-accelerated)

## 🔎 Project Workflow

### 1. Data Exploration and Preparation
- Load dataset
- Clean, scrape, and preprocess content

### 2. Environment Setup
- Install dependencies using `requirements.txt`
- Set runtime to GPU for efficiency

### 3. Model Development
- Implement custom:
  - Dataset class
  - DataLoader
  - BART summarization logic using `BARTForConditionalGeneration`

### 4. Model Training
- Split data into train/test sets
- Fine-tune the model using a custom trainer

### 5. Summarization and Evaluation
- Generate summaries with the model
- Evaluate using ROUGE metrics:
  - **ROUGE-1** (unigram)
  - **ROUGE-2** (bigram)
  - **ROUGE-L** (longest common subsequence)

### 6. Web Application Deployment
- Flask-based interface to input and summarize articles
- Run locally and access via browser

## 📁 Project Structure

```
.
├── data/                # Raw and processed data
│   └── news_articles.csv
├── src/                 # Core model and utilities
│   ├── bart_summarization.py
│   ├── dataset_loader.py
│   └── trainer.py
├── app/                 # Flask web app
│   └── app.py
├── output/              # Model outputs and metrics
├── requirements.txt     # Project dependencies
└── README.md            # Project documentation
```

## ▶️ Getting Started

```bash
# Clone the repository
git clone <repository_url>
cd <repository_folder>

# Install dependencies
pip install -r requirements.txt

# Run the summarization model
python src/bart_summarization.py

# Launch the web application
cd app/
python app.py
```

Open your browser and go to [http://127.0.0.1:5000](http://127.0.0.1:5000)

## ✅ Results

- ✅ High-quality, abstractive summaries  
- ✅ Competitive ROUGE scores  
- ✅ Simple, user-friendly web interface

## 🤝 Contributing

We welcome your contributions!

```bash
# Fork and clone the repository
git checkout -b feature-name

# Make your changes
git commit -m "Add feature"

# Push and open a pull request
git push origin feature-name
```

## 📄 License

Licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

## 📬 Contact

**👤 Abhinav Navneet**  
📧 mailme.AbhinavN@gmail.com  
🐙 GitHub: [AjNavneet](https://github.com/AjNavneet)

## 🙌 Acknowledgments

- Hugging Face  
- Google Colab  
- PyTorch  
- Python Open Source Community
