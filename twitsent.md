## Towards Real-Time Monitoring of Public Opinion on Twitter Using Sentiment and Emotion Analysis

### Introduction 

The goal of this project is to create a real-time machine learning system for analyzing sentiment and emotions in tweets from Twitter. It differentiates between sentiment, which reflects the overall attitude or opinion, encompassing positive and negative expressions, and emotions, encompassing complex psychological states like happiness, sadness, anger, and fear. The research aims to develop a methodology that combines sentiment and emotion analysis to offer a deeper understanding of public sentiment on Twitter, providing more nuanced insights into user opinions.

### Data

NLTK and vader_lexicon was used for sentiment analysis, SemEval 2018 - Task E-c dataset for emotion classification, and applied extensive preprocessing. The Twitter dataset, collected using specific keywords, includes at least 50,000 tweets per topic and underwent preprocessing.

<img src="images/joywordcloud.jpg?raw=true"/>
A word cloud generated from tweets labeled with the emotion "joy".

### Methodology

The project comprises three key phases: 
<br>
<br>
In Part 1, we collect COVID-19-related tweets and employ NLTK for sentiment analysis. The sentiment trends are then visualized over time, providing insights into public opinion evolution.
<br>
<br>
Part 2 involves training a machine learning model to classify emotions in tweets using the SemEval dataset. We adapt the sentiment analysis algorithm for emotion identification, encompassing pre-processing, text vectorization, and machine learning model training. ML methods include BernoulliNB, LogisticRegression, and LinearSVC.
<br>
<br>
In Part 3, we collect tweets related to specific topics like Covid-19 and ChatGPT. A tool is deployed to classify real-time tweets and plot sentiment and emotion changes over time, allowing us to understand the evolving public opinion on different topics.

### Results

**Relating emotions to sentiments**
  The sentiment and emotion pairs' scores are calculated by summing their strengths when they co-occur in tweets. This information is visualized in a bipartite graph, where edge thickness represents the pair's weight, and this process is repeated for both "covid" and "chatGPT" topics.

<img src="images/bipartite.jpg?raw=true"/>


**Estimating sentiments and emotions in real-time:**
  To monitor the live Twitter stream, we filter relevant tweets using keywords. Then, we analyze sentiment and emotions by running the NLTK classifier and machine learning models on sets of 20 consecutive tweets. This data is used to update a dynamic plot tracking changes in sentiment and emotions over time.

<img src="images/twitsent.jpg?raw=true"/>

### Conclusion

The project aims to develop a real-time machine learning approach for sentiment and emotion analysis of Twitter data. This involves pre-processing, text vectorization, and machine learning model training to classify emotions in tweets. By linking emotions to sentiments and filtering live Twitter streams with user-provided keywords, it offers nuanced insights into public opinion. Ultimately, this project can provide a powerful real-time tool for monitoring public sentiment on various topics.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
