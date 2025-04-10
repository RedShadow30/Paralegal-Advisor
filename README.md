# Paralegal Advisor

### Introduction ⚖️
Paralegals navigate an overwhelming number of documents and past cases to find information strengthening their argument. Their responsibilities of conducting research and organizing facts can be streamlined using a combination of question answering (QA) and sentiment analysis.  

#### Our Vision 👀
Our goal was to minimize the overhead involved during legal research. We aim to provide legal experts with a tool that allows them to gather information efficiently.

### Overview
- Question Answering: User provides case document and a prompt such as "Why was the accused charged with death penalty?" Returns extracted answer from the case document.
- Semantic Search: User provides case overview. Returns most similar past cases using MongoDB's vector search index.
- Sentiment Analysis: Classifies a piece of text as positive or negative based on the words used. Positive represents a won case and negative represents a lost case.

Bonus (Future Implementation):
- Contextual Summarization: Examines a case to highlight key arguments established and reference to applicable laws. 

### Dataset 📚
QA: Legal Dataset
Sentiment Analysis: IMDB

### TODO: Methodology 🎯
Data Ingestion: web scrape, Kaggle/HF dataset imports
Preprocessing: text normalization, stopword removal, punctuation removal, HTML tag removal
Visualizations:
Transformers Used:
Statistical Models Used:
...

### TODO: Findings 📊
TBD