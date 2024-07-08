# Information-Retrieval-System
Developed an information retrieval system that fetches relevant city descriptions based on user queries using natural language processing techniques and cosine similarity for accurate and efficient travel information.

Steps Involved
Importing Libraries: Necessary libraries such as json, pandas, nltk, TfidfVectorizer, and cosine_similarity were imported.

Loading JSON Data: The JSON data was loaded from a specified file path.

Extracting City Names and Descriptions to create a DataFrame: City names and their corresponding descriptions were extracted from the JSON data to create a DataFrame with the columns city , description.

Checking for Duplicates: Duplicates in the city names column were checked.

Downloading NLTK Resources: Necessary NLTK resources such as 'punkt', 'averaged_perceptron_tagger', and 'stopwords' were downloaded.

Defining Stop Words: English stop words were defined using NLTK's stop words corpus.

Preprocessing Text: A function was created to preprocess text by lowercasing stop words and all words except nouns. Parts of speech (POS) tagging was used to identify nouns.

Applying Preprocessing: The preprocessing function was applied to the descriptions in the DataFrame.

TF-IDF Vectorization: The TF-IDF vectorizer was initialized and fit on the cleaned descriptions.

Retrieving Relevant Cities: A function was defined to retrieve relevant cities based on the user query. The query was preprocessed, transformed using the TF-IDF vectorizer, and cosine similarity was calculated to find the most relevant cities.

Example Usage: Example queries were provided to demonstrate the functionality of the information retrieval system.
