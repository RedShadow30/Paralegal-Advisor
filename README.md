# Paralegal Advisor

### Introduction ⚖️
Paralegals navigate an overwhelming number of documents and past cases to find information strengthening their argument. Their responsibilities of conducting research and organizing facts can be streamlined using a combination of question answering (QA) and sentiment analysis.  

#### Our Vision 👀
Our goal was to minimize the overhead involved during legal research. We aim to provide legal experts with a tool that allows them to gather information efficiently.

### Overview
- Question Answering: User provides case document and a prompt such as "Why was the accused charged with death penalty?" Returns extracted answer from the case document.
- Semantic Search: User provides case overview. Returns most similar past cases using MongoDB's vector search index.
- Sentiment Analysis: Classifies a piece of text as positive or negative based on the words used. Positive label represents a won case and negative label represents a lost case.

[Project Workflow](https://drive.google.com/file/d/17SBYihxCSsiTUQqeIgyEdN30pzHwtLy6/view?usp=sharing) - by @RedShadow30

Bonus (Future Implementation):
- Contextual Summarization: Examines a case to highlight key arguments established and reference to applicable laws. 

### Dataset 📚
QA: Legal Dataset
Sentiment Analysis: Stanford IMDB Dataset

### Methodology 🎯
Data Ingestion: Web scrape, Kaggle/HF dataset imports

Preprocessing: Text normalization, Stopword removal, Punctuation removal, HTML tag removal

Visualizations: Pie-Chart, Bar Graphs, Line Graphs, Word Cloud

Transformers Used: BERT, RoBERTa, DistilBERT

Statistical Models Used: Decision Tree and Random Forest

### Findings 📊
- Manipulating the duplicate words within the data for Question answering helped the model avoid returning repetitive words within it's extracted answer.
- RoBERTa had the highest F1 and EM scores for Question Answering. Then, DistilBERT and BERT, respectively.
- Most cases were classified as Negative for sentiment analysis.
- It was difficult for the IMDB trained transformers to conclude the case sentiment based on the words in the case text. This was due the high usage of negative words in the text. 

#### TF-IDF

![TF_IDF](images/tfidf.png)


#### Question Answering:
BERT

![BERT Finetuned Results](images/image.png)

DistilBERT

![DistilBERT Finetuned Results](images/image-1.png)

RoBERTa

![RoBERTa Finetuned Results](images/image-2.png)

#### Sentiment Analysis:

DistilBERT

![DistilBERT SA Results](images/db-sa.png)

BERT

![BERT SA Results](images/bertsa.png)

### Meet the Team 😎 

@JaidynGreen01 - BERT
@GustavoPlatas22 - RoBERTa
@OzielPlatas - RoBERTa
@RedShadow30 - DistilBERT

### Thank You!