# News Articles Title Generation (INF582)

## Introduction

The primary objective of this challenge is to use and develop advanced natural language processing (NLP) models to automatically generate compelling and informative titles for news articles. this project was carried out as part of the evaluation of the "Introduction to Text Mining and NLP" course, given by Michalis Vazirgiannis at Ecole Polytechnique.

In today's fast-paced digital age, the sheer volume of news articles published daily can be overwhelming for readers. An effective headline serves as a crucial gateway that influences whether readers click to access the full article. Automated title generation not only streamlines the content creation process for publishers but also ensures that readers quickly grasp the core message of an article. This challenge aims to improve user experience, enable efficient information consumption, and contribute to the evolution of news dissemination in the digital realm.

### Dataset Description

The dataset contains French news articles with various topics. We were provided with the following files:

1. `train.csv`: Contains 30,659 news articles and their titles.
2. `validation.csv`: Contains 1,500 news articles and their titles.
3. `test_text.csv`: Contains 1,500 news articles for which you need to generate titles.

Ensure that your submissions follow the provided format (ID, titles) to be accepted by Kaggle.

### Evaluation

The performance of our models has been assessed using the ROUGE-L F-Score metric. ROUGE evaluates the overlap between the generated title and reference titles using n-grams and the Longest Common Subsequence (LCS).

### Provided Source Code

We were given a Python script with basic extractive summarization baselines:

- **Lead-1**: Extracts the first sentence of the input text as the title. This method assumes the opening sentence encapsulates the main idea.
- **EXT-ORACLE-1**: Uses original titles to identify the most salient information for generating titles.

### Models Developed

For this project, we have developed the following models:

- **Custom Encoder-Decoder Model**: Utilizes an encoder-decoder structure with LSTM layers and a global attention mechanism to generate news article titles.
- **Fine-Tuned Large Language Models**: We have fine-tuned existing LLMs such as BERT and T5 from **[Hugging Face](https://huggingface.co/)** to improve title generation performance.

### Collaborators

This project was developed by the following team members:

- **[Maxime Moutet](https://www.linkedin.com/in/maximemoutet)**
- **[Paco Goze](https://www.linkedin.com/in/paco-goze-086515174)**
- **[Samuel Gaudin](https://www.linkedin.com/in/samuel-gaudin/)**
