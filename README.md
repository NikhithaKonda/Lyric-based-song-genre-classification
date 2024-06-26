# Lyric- Based-Song-Genre-Classification

## Authors
Nikhitha Konda

Kartheik Duggirala

## Introduction
Identifying music genres through lyrics has gained prominence in music research. It's crucial for enhancing music recommendation systems and search engines. Genres, defined by tempo, melody, instrumentation, and lyrics, offer insights into a song's mood and themes. This study explores rock, pop, and hip hop lyrics using NLP techniques like tokenization, stemming, and stop word removal, alongside TF-IDF, BERT, GLOVE, and Word2Vec. ML models such as Random Forest, Gradient Boosting, Naive Bayes, MLP, Logistic Regression, KNN, SVM, LSTM, and CNN are employed for classification. LSTM proves most effective. These findings benefit music recommendation accuracy and genre classification in various applications.

## Data Acquisition
The project faces a major challenge in gathering data to construct the LSTM model. Copyright constraints and the lack of publicly available datasets across various music genres led to the decision to extract lyrics from Musixmatch.com through web scraping. This website was selected for its accurate and diverse lyric content, as well as its cost-free accessibility. However, web scraping necessitates careful consideration of legal and ethical implications. The team commits to adhering to all regulations during data extraction, ensuring relevance and representation of diverse music genres. Additionally, they discovered a suitable lyrics dataset on GitHub, which was merged based on genres. Efforts are focused on acquiring high-quality, reliable data crucial for building the LSTM model.

## Machine Learning Models Used
We tested seven machine learning models on the data, finding that Ensemble learning algorithms outperformed others, followed by Logistic Regression and MLP classifier. Initially, we used TF-IDF to convert text into numerical vectors for model input. Despite experimenting with pre-trained models like Word2Vec and Glove, TF-IDF yielded higher accuracy. Specifically, Random Forest with TF-IDF excelled over pre-trained word embedding models according to the chart.

## Analysis and Results 
After experimenting with machine learning models, neural networks were tested, including CNN and LSTM, with Tokenizer from Keras, Bert, and Glove models. CNN accuracy improved with pre-trained models, while LSTM accuracy decreased. LSTM with tokenization achieved the highest accuracy compared to Glove and BERT. Overall, base models outperformed pre-trained ones.
The model architecture comprises an embedding layer, an LSTM layer, and a dense layer with softmax activation. Trained for 10 epochs using Adam optimizer and categorical cross-entropy loss on a training set. LSTM excels in NLP due to its ability to handle long-term dependencies via memory cells, beneficial for tasks like language translation and text generation. Its success extends to music-related tasks like genre classification, offering comprehensive context understanding and noise tolerance in lyrics. However, it requires ample labeled data for optimal performance, which can be mitigated by large datasets like the Million Song Dataset (MSD).
