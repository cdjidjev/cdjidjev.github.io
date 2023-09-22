## Towards Real-Time Monitoring of Public Opinion on Twitter Using Sentiment and Emotion Analysis

**Introduction:** 
The aim of this project is to develop a machine learning-based approach to analyze sentiment and emotions in tweets from Twitter in real-time.
  • Sentiment vs emotions: related concepts but have distinct meanings.
  • Sentiment: refers to the general attitude or opinion towards
  something
      o Positive: “it is a nice place,” “food was tasty”
      o Negative: “had a terrible experience,” “I hated the movie”
  • Emotions: complex psychological states such as happiness, sadness, anger, and fear.
This research project aims to develop a methodology that leverages both sentiment and emotion analysis to provide more nuanced insights into public opinion on Twitter.

### Data

• Data is needed in order to inform the classification model about how words in a tweet determine the type and intensity of sentiment or emotion.
• Sentiment analysis data: The Natural Language Toolkit (NLTK) datasets and the vader_lexicon were used as the primary approach for sentiment analysis. vader_lexicon provides a set of lexical features that can be used to determine the sentiment of a piece of text by identifying positive or negative sentiment words.
• Emotions analysis data: SemEval 2018 - Task E-c: This dataset is used to train the emotion classification models. It contains 20,000 tweets that were manually labeled as either 'neutral or no emotion' (0) or as one (1) of eleven emotions, including anger, anticipation, disgust, fear, joy, love, optimism, pessimism, sadness, surprise, and trust. The dataset was obtained from Kaggle.com and underwent extensive preprocessing steps: cleaning and removing punctuation, repeating characters, URLs, numbers, stop words, applying lemmatization, tokenization, reducing words to their stem, base, or root, and finally converting into the IF-TDIF format.
• Twitter data: Dataset consists of tweets collected using the Twitter API using a set of rules (keywords) related to topic of interest. It contains at least 50,000 tweets per topic and includes information on the tweet message, author, and time/date posted. The dataset was pulled using the official Twitter API and the filtered stream endpoint and underwent preprocessing steps. Used keywords “covid” and “chatGPT”.


### Methodology

The project can be divided into three parts:
Part 1: Sentiment
  • Collect a set of tweets related to COVID-19
  • Analyze their sentiment using the NLTK library
  • Plot the sentiment changes over time to gain
insights into how public opinion on the topic
has evolved.
Part 2: Emotions
  • Train a machine learning model to classify emotions in tweets.
  • Use SemEval dataset to train the model.
  • Adapt the sentiment analysis algorithm
  to identify emotions in tweets.
  • The methodology involves:
      o Pre-processingthetweets
      o Vectorizingthetext
      o Trainingthemachinelearningmodel
A word cloud generated from tweets labeled with the emotion "joy".
ROC curve for emotion "joy” and ML method “LinearSVC”.
to classify emotions in the tweets
      o MLmethodsused:BernoulliNBv,LogisticRegression,LinearSVC
Part 3: Putting it together and deploying on the live twitter stream
  • Collect twitter data based on a topic; for this project we chose Covid-19 and ChatGPT.
  • Deploy the tool on a filtered streaming Twitter endpoint to classify incoming tweets in real-time.
  • Plot the sentiment and emotion changes over time for each topic.
  • Gain insight into how public opinion evolves based on different topics.

### Results

**Relating emotions to sentiments**
  • Check how each emotion relates to positive and/or negative sentiments.
  • For each sentiment type and emotion pair, if they appear in the same tweet,
  add their strength sum to the pair score.
  • Display the information as a bipartite graph, where the thickness of each edge
  encodes the weight of the corresponding pair computed in the previous step
  • Do for each topic (covid or chatGPT).

**Estimating sentiments and emotions in real-time:**
  • Filter tweets from the live Twitter stream that match the keyword(s).
  • On each set of 20 consecutive tweets,
  • Run the NLTK classifier to get positive and negative sentiment scores.
  • Determine the strength of each emotion e by running the ML model for e.
  • Update a dynamic plot that shows how the sentiment and emotions change
  over time.

<img src="images/dummy_thumbnail.jpg?raw=true"/>

### 4. Conclusion

• The project aims to develop a machine learning-based approach to analyze sentiment and emotions in tweets from Twitter in real-time.
• Leveraging both sentiment and emotion analysis provides more nuanced insights into public opinion on Twitter.
• The methodology involves pre-processing the tweets,vectorizing the text,and training the machine learning model to classify emotions in the tweets.
• Our analysis also relates emotions to sentiments and estimates sentiments and emotions in real-time by filtering tweets from the live Twitter stream that match user-provided keywords,
• The project can contribute to the development of a powerful tool that helps monitor public opinion on a range of topics in real-time.

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
