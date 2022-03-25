![download](https://user-images.githubusercontent.com/68982975/160054636-d3b66d29-2feb-493f-bd56-00b4092d5c30.jpeg) ![download](https://user-images.githubusercontent.com/68982975/160054523-034b2c5c-4bb6-4667-9db4-70d275fc95f0.png)


### More than a five-star rating: E-commerce Customer Review Analysis




**Abstract**

Understanding customers is important for a business to reflect what customers need and to help increase profits. The goal of this project was to predict and distinguish positive and negative reviews of customers and to analyze what customers complain about. I used [Amazon Reviews](https://www.kaggle.com/datasets/kritanjalijain/amazon-reviews) found on Kaggle. To forecast whether customer reviews were either negatively or positively written,  I used Bidirectional LTSM and GRU and achieved .82 accuracy scores. Customers’ complaints are categorized by using an LDA model into 32 topics. 


**Design**

For the sentiment analysis, I predicted whether customer text reviews were positive or negative using deep learning techniques (i.e., RNN). After comparing deep learning models to my baseline model, a GRU model outperformed the baseline model with Random Forest and LTSM model. 

Next, an LDA model was used to analyze and summarize what customers complained about products after text preprocessing. TF-IDF and bi-trigram improved the model performance than CountVectorizer with unigram. The number of the topic was decided by looking at the coherence score. 


**Data**

The Amazon Reviews dataset includes a total of 3.6M documents. In this project, I selected a set of 71998 random documents for the sentiment analysis and 5998 documents for topic modeling due to the memory space of my computer CPU.


**Tools**

- Tensorflow & Keras 
- Sklearn
- Spacy 
- Gensim
- NLTK
- PyLDAvis
- Matplotlib
- WordCloud


**Future studies**

- More hyperparameter tuning is necessary (such as optimizer and activation functions) to overcome the overfitting issue and improve the accuracy score
- Due to the large text data size, I partially analyzed the negative reviews, so it turned out to be only complaints of books and movies. Using the entire dataset may yield different results and interpretations. Thus, tuning hyperparameter and rerunning with the entire data is necessary to see other types of complaints on other product types.
