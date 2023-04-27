# Gender Bias and Cultural Journalism: Article Classification using Natural Language Processing and Machine Learning Algorithms
Jupyter notebook in support of the work for my final paper 2023, which consists of the following:

- training a word2vec algorithm on a dataset of articles collected from the New York Times related to culture ("cultural journalism")
- evaluation of a gender bias coefficient for each article based on the cosine similarity between the average word embedding representing the article and the gender dimension in the corpus 
- textual feature extraction (headline, lead paragraph)
- training of three classification algorithms to classify articles into sections (softmax classifier, random forest classifier, multi-layer perceptron) on both the original imbalanced dataset and the oversampled dataset (due to high dataset imbalance)
- based on the best-performing algorithm (random forest classifier, 95% accuracy on the balanced dataset), evaluation of SHAP values to determine gender bias coefficient feature importance

The repo contains also a second notebook: Headline Sentiment Analysis. This notebook was developed for the appendices of the paper. It contains:
- author gender prediction based on the author's first name
- headline sentiment analysis using RoBERTa embeddings from a model trained on Twitter corpora to perform polarity score identification
- OLS regression to evaluate statistical importance of author gender in explaining polarity score (example with negative polarity score)

*Note*: Jupyter notebooks I developed to scrape the New York Times and collect the dataset can be found at this [repository](https://github.com/susannapaoli/web-scraper-nyt)
