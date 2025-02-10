# NLP Digital Content Management
Build a sequential NLP classifier to determine customer sentiments, identify the labels of blogs, and create a chatbot. 
### **In Part 2 the chatbot named "*Olywalker*" is created and it gives satisfactory responses to the questions asked.**

**• DOMAIN:** Digital content and entertainment industry
## PART 1

**• CONTEXT:** 

The objective of this project is to build a text classification model that analyses the customer's sentiments based on their reviews in the IMDB database. The model uses a complex deep learning model to build an embedding layer followed by a classification algorithm to analyze the sentiment of the customers.

**• DATA DESCRIPTION:** 

The Dataset of 50,000 movie reviews from IMDB, labeled by sentiment (positive/negative). Reviews have been preprocessed, and each review is encoded as a sequence of word indexes (integers). For convenience, the words are indexed by their frequency in the dataset, meaning the one that has index 1 is the most frequent word. Use the first 20 words from each review to speed up training, using a max vocabulary size of 10,000. As a convention, "0" does not stand for a specific word, but instead encodes any unknown word.


**• OBJECTIVE**: 

Build a sequential NLP classifier that can use input text
parameters to determine the customer sentiments.

**• Steps and tasks:**
1. Import and analyze the data set.
  - Use `imdb.load_data()` method
  - Get train and test set
  - Take 10000 most frequent words
2. Perform relevant sequence padding on the data
3. Perform data analysis:
  - Print the shape of features and labels
  - Print value of any one feature and its label
4. Decode the feature value to get the original sentence
5. Design, train, tune, and test a sequential model.

The aim here Is to import the text and process it in such a way that it can be taken as input to the ML/NN
classifiers. 
6. Use the designed model to print the prediction on a sample.

**• CONCLUSION :**
- **The model using Glove Embeddings is performing better with 84 % accuracy.**

- **From the confusion matrix we can observe that 3965 reviews are correctly classified as Non-Sarcastic (True Negative) and 3014 reviews are correctly classified as Sarcastic (True Positive).**

- **The model also has better Recall  (86 %) and F1 Score (83 %).**


## *****************************************************************************************************************************
## PART 2

**• CONTEXT:**

Classification is the most popular task that we deal with in real life. Text in the form of blogs, posts, articles, etc. is written every second. It is a challenge to predict the information about the writer without knowing about him/her. We are going to create a classifier that predicts multiple features of the author of a given text. We have designed it as a Multi-label classification problem.

**• DATA DESCRIPTION:**

Over 600,000 posts from more than 19 thousand bloggers The Blog Authorship Corpus consists of the collected posts of 19,320 bloggers gathered from blogger.com in August 2004. The corpus incorporates a total of 681,288 posts and over 140 million words - or approximately 35 posts and 7250 words per person. Each blog is presented as a separate file, the name of which indicates a blogger ID # and the blogger’s self-provided gender, age, industry, and astrological sign. (All are labeled for gender and age but for many, industry and/or sign is marked as unknown.) All bloggers included in the corpus fall into one of three age groups:

• 8240 "10s" blogs (ages 13-17),

• 8086 "20s" blogs(ages 23-27) and

• 2994 "30s" blogs (ages 33-47)

For each age group, there is an equal number of male and female bloggers.

Each blog in the corpus includes at least 200 occurrences of common English words. All formatting has been stripped with two exceptions.
Individual posts within a single blogger are separated by the date of the following post and links within a post are denoted by the label url link.

Link to dataset: 
`https://www.kaggle.com/rtatman/blog-authorship-corpus`

**• PROJECT OBJECTIVE**:

To build an NLP classifier that can use input text parameters to determine the label/s of the blog.

**• Steps and tasks:**
1. Import and analyze the data set.
2. Perform data pre-processing on the data:

  -Data cleansing by removing unwanted characters, spaces, stop words, etc. Convert text to lowercase.
  -Target/label merger and transformation
  -Train and test split
  -Vectorisation, etc.

3. Design, train, tune, and test the best text classifier.
4. Display the classification report
5. Print the true vs predicted labels for any 5 entries from the dataset.

   **• CONCLUSION :**

   **Designed a Python-based interactive semi-rule-based chatbot that can do the following:**
  - Start the chat session with greetings and ask what the user is looking for.
  - Accept dynamic text-based questions from the user. Reply with a relevant answer from the designed corpus.
  - End the chat session only if the user requests to end else ask what the user is looking for. The loop continues till the user asks to end it.

