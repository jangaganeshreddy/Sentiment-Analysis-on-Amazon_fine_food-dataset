# Sentiment-Analysis-on-Amazon_fine_food-dataset
# Objective: 
The objective of this project was to perform sentiment analysis on the “Amazon Fine Food Reviews” dataset using transformer models.
# DataSet Used: 
The “Amazon Fine Food Reviews” dataset was chosen for this project. This dataset is publicly available on Kaggle and contains text reviews of food products on Amazon, along with the rating (score) given by the reviewer. The dataset is well-suited for sentiment analysis as it provides real-world, user-generated text data along with a numerical indicator (the score) of the sentiment expressed in each review.

Link: 

# Model Architecture: Two different models were used for sentiment analysis in this project:

**VADER (Valence Aware Dictionary and sEntiment Reasoner)**: VADER is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media. It uses a bag-of-words approach, where each word in the text is scored for its sentiment, and these scores are combined to give a total sentiment score for the text.

**RoBERTa (A Robustly Optimized BERT Pretraining Approach):** RoBERTa is a transformer model that is based on BERT (Bidirectional Encoder Representations from Transformers). It was used in this project in a pretrained form, loaded from Hugging Face’s model hub. The model takes tokenized text as input and outputs a sentiment label.

# Implementation Process and Challenges: 
The implementation process involved several steps, including data loading, data preprocessing, model application, and result visualization. One of the main challenges faced during implementation was the computational cost of applying the RoBERTa model to each review in the dataset. To handle this, exceptions were caught and handled in the loop to prevent the entire process from breaking due to a single problematic review.

# Model Evaluation: 
The sentiment scores from VADER and RoBERTa were compared visually using pairplots. The sentiment scores seemed to align well with the Amazon review scores, indicating that both models were able to capture the sentiment expressed in the reviews to some extent. However, a more detailed evaluation (e.g., calculating accuracy, precision, recall, F1 score, etc.) would provide a more quantitative measure of the models’ performance.
