## Towards Real-Time Monitoring of Public Opinion on Twitter Using Sentiment and Emotion Analysis

The primary objective is to build a real-time machine-learning system for sentiment and emotion analysis of Twitter data, employing natural language processing using *NLTK* and *vader_lexicon* for sentiment analysis, utilizing the *SemEval 2018 - Task E-c* dataset for emotion classification, and *scikit-learn* and *matplotlib* python libraries among others. The project encompasses extensive data preprocessing, text vectorization, and machine learning model training, including methods like BernoulliNB, LogisticRegression, and LinearSVC. 

The project consists of the following parts: 
- SOMETHING ABOUT COLLECTING AND STORING TWEETS FROM STREAMING ENDPOINTS on specific topics
- sentiment trend analysis over time (WHAT ARE THE SENTIMENTS), 
- emotion identification over time (WHAT ARE THE EMOTIONS), and
- real-time sentiment and emotion relationship analysis.

The results are visualized as bipartite graphs and dynamic plots, providing insights into evolving public opinion. The following figures were created using tweets pulled with the keywords "covid" and "chatGPT". In this first image, we have a bipartite graph that shows the relationships between negative or positive sentiment and each of the emotions. The thickness of the edge encodes the weight of the corresponding pair.

<img src="images/bipartiteCovid.jpg?raw=true"/>


Next we have a dynamic plot showing average change of emotions per batch of tweets over time and a dynamic pie chart showing frequency of emotions per batch of tweets over time. 

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/12867180-6878-451b-b62d-1dfe56cd94e9" controls="controls" style="max-width: 500px;">
</video>

<video src="https://github.com/cdjidjev/cdjidjev.github.io/assets/40774209/7223d7d6-0841-4c0e-a28b-841bdbfd96e1" controls="controls" style="max-width: 500px;">
</video>





Ultimately, this project aims to offer a powerful real-time tool for tracking sentiment and emotions across various Twitter topics..


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
