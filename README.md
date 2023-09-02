# ML Book Genre Classifier

# A model using TD-IDF to predict the genre of 3000 books based on their summary.

Project Overview:

This GitHub repository hosts a supervised Machine Learning (ML) project aimed at classifying book genres based on their blurbs. The project encompasses several key steps to achieve this classification:

Data Preprocessing:

The dataset is cleaned, including the removal of unnecessary columns.
A text cleaning function is employed to remove special characters, tabs, and spaces while converting text to lowercase.

Exploratory Data Analysis (EDA):

An EDA function is created to display the 'n' most frequent words in the form of a bar graph using FreqDist() from the Natural Language Toolkit (NLTK).

Text Preprocessing:

Stopwords (commonly occurring but insignificant words) are removed from the text, enhancing the relevance of the remaining words.

Frequency of words before removing stopwords:

<img width="369" alt="image" src="https://user-images.githubusercontent.com/88050198/211047786-d999fb6f-045a-46e5-a9e1-738f56f334f5.png">

Frequency of words after removing stopwords (one can see more useful/meaningful words):

<img width="411" alt="image" src="https://user-images.githubusercontent.com/88050198/211047846-01ce1f4e-5332-4c23-b57d-677bf6cf85ce.png">

Lemmatization vs. Stemming:

Lemmatization, a text normalization technique, is applied to convert words to their base root form. Unlike stemming, lemmatization considers context, making it more suitable for this project.
Stemming is briefly discussed and deemed less appropriate due to the need for context in book genre prediction.

Feature Extraction:

Count Vectorization is utilized to convert strings into a frequency representation.
TF-IDF (Term Frequency — Inverse Document Frequency) is explained as a superior alternative to Count Vectorization. TF-IDF not only captures word frequency but also their importance.

Machine Learning Models:

The project employs Support Vector Classification (SVC), which is based on libsvm, as one of the classification algorithms.
Multinomial Naive Bayes is highlighted as a suitable classifier for this project due to its compatibility with discrete features, such as word counts in text.

Results of the predicted genres vs original genres

<img width="320" alt="image" src="https://user-images.githubusercontent.com/88050198/211049567-d285ec05-39e8-4d14-b5fc-4f8e8af122f6.png">

<img width="316" alt="image" src="https://user-images.githubusercontent.com/88050198/211049603-5b8c215b-894a-47a7-9622-0533cab960c0.png">

Please feel free to explore this repository for in-depth insights into the project, including code, datasets, and model evaluations.
