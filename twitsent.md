## Towards Real-Time Monitoring of Public Opinion on Twitter Using Sentiment and Emotion Analysis

The primary objective is to build a real-time machine-learning system for sentiment and emotion analysis of Twitter data, employing natural language processing using *NLTK* and *vader_lexicon* for sentiment analysis, utilizing the *SemEval 2018 - Task E-c* dataset for emotion classification, and *scikit-learn* and *matplotlib* python libraries among others. The project encompasses extensive data preprocessing, text vectorization, and machine learning model training, including methods like BernoulliNB, LogisticRegression, and LinearSVC. 

The project consists of the following parts: 
- Retrieve tweets from Twitter's API using a filtered stream endpoint with a predefined set of rules (keywords),
- sentiment (negative or positive) trend analysis over time, 
- emotion (joy, optimism, love, fear, pessimism, anger, anticipation) identification over time, and
- real-time sentiment and emotion relationship analysis.

<!-- The results are visualized as bipartite graphs and dynamic plots, providing insights into evolving public opinion. -->
The following figures were created using tweets pulled with the keywords "covid" and "chatGPT" on April 14th 2023 at 11:46am - April 14th 2023 at 1:03pm. 

- **Relationships between sentiments and each of the emotions:** The thickness of the edge encodes the weight of the corresponding pair.

keyword: "covid"
<p align="center"  width="500">
<img src="images/bipartiteCovid.jpg?raw=true"/>
</p><br><br>

- **Emotions magnitudes over time:** The dynamic plot shows average change of emotions over the time period of about half of an hour. 

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/12867180-6878-451b-b62d-1dfe56cd94e9" controls="controls" style="max-width: 500px;">
</video>
<br><br>

- **Emotions dynamics as a pie chart:**  The dynamic pie chart shows the relative frequency of emotions over the same period of time, where tweets data is divided into 100 batches. 

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/7223d7d6-0841-4c0e-a28b-841bdbfd96e1" controls="controls" style="max-width: 500px;">
</video>
<br><br>

Ultimately, this project is a step towards building a powerful real-time tool for dynamically tracking sentiment and emotions across various Twitter topics.

