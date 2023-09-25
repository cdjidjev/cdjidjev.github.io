## Towards Real-Time Monitoring of Public Opinion on Twitter Using Sentiment and Emotion Analysis

In this data science project, the primary objective is to build a real-time machine learning system for sentiment and emotion analysis of Twitter data. This involves skills such as natural language processing using NLTK and vader_lexicon for sentiment analysis, as well as utilizing the SemEval 2018 - Task E-c dataset for emotion classification. The project encompasses extensive data preprocessing, text vectorization, and machine learning model training, including methods like BernoulliNB, LogisticRegression, and LinearSVC. For example below is a word cloud generated from tweets labeled as having the emotion 'joy'. The bigger the word, the more frequently it occured in that set of tweets. 

<img src="images/joywordcloud.jpg?raw=true"/>

The project is divided into three phases: sentiment trend analysis over time, emotion identification using machine learning, and real-time sentiment and emotion monitoring on specific topics. The results are visualized in bipartite graphs and dynamic plots, providing valuable insights into evolving public opinion. 

The following figures were created using tweets pulled with the keywords "covid" and "chatGPT". In this first image we have a bipartite that shows the relationships between negative or positive sentiment and each of the emotions. The thickness of the edge encodes the weight of the corresponding pair.

<img src="images/bipartiteCovid.jpg?raw=true"/>


Next we have a dynamic plot showing average change of emotions per batch of tweets over time and a dynamic pie chart showing frequency of emotions per batch of tweets over time. 

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/12867180-6878-451b-b62d-1dfe56cd94e9" controls="controls" style="max-width: 500px;">
</video>

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/7223d7d6-0841-4c0e-a28b-841bdbfd96e1" controls="controls" style="max-width: 500px;">
</video>





Ultimately, this project aims to offer a powerful real-time tool for tracking sentiment and emotions across various Twitter topics..


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
