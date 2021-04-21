# Fake-News-Detection
This project aims to detect pieces of news that may be hoaxes and are generally spread through social media and other online media. Such news items may contain false and/or exaggerated claims, and may end up being viralized by algorithms, and users may end up in a filter bubble.

In this project, I am using TfidfVectorizer to convert the collection of raw documents into a matrix of TF-IDF features.
TF (Term Frequency): The number of times a word appears in a document is its Term Frequency. A higher value means a term appears more often than others, and so, the document is a good match when the term is part of the search terms.
IDF (Inverse Document Frequency): Words that occur many times a document, but also occur many times in many others, may be irrelevant. IDF is a measure of how significant a term is in the entire corpus.

I am using Passive Aggressive Classifier to train my model and was able to achive 95.95% accuracy. Passive Aggressive algorithms are online learning algorithms. Such an algorithm remains passive for a correct classification outcome, and turns aggressive in the event of a miscalculation, updating and adjusting. Unlike most other algorithms, it does not converge. Its purpose is to make updates that correct the loss, causing very little change in the norm of the weight vector.

I downloaded the train and test datasets from Kaggle: https://www.kaggle.com/c/fake-news/data
Because the train dataset is too big. I could not upload it here.
