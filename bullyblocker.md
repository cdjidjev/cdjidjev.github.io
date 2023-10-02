# BullyBlocker Project Summary Report

## Introduction

Over the course of three semesters, our interdisciplinary project at Arizona State University, known as BullyBlocker, focused on researching and developing methods to extract and analyze data from the social network platform TikTok, with the goal of identifying and addressing instances of cyberbullying. This report outlines my key activities and findings throughout the project.

## Semester 1: Data Extraction from TikTok

In the initial semester, my primary focus was on data extraction from TikTok:

1. **Researching TikTok Data Extraction**: I delved into various methods to extract data from TikTok, understanding its data structure and the challenges it presented.

2. **API Exploration**: I scoured the web for APIs that could provide access to TikTok data, and identified two APIs, one free and one paid, that offered the potential to retrieve data regarding sessions, authors, keywords, comments, and more.

3. **Code Implementation**: Using the TikTokAPI module, I wrote and implemented code to extract sessions (TikTok videos) based on specific keywords.

4. **Keyword Analysis**: I retrieved sessions containing a predefined list of 25 keywords relevant to cyberbullying and saved these sessions to disk for further analysis.

5. **Sorting Sessions**: I developed a method to sort sessions based on the number of cyberbullying keywords they contained.

6. **Comments Retrieval**: I also created a method to retrieve a specified number of comments from selected sessions.

## Semester 2: Data Analysis and Challenges

During the second semester, my focus shifted toward data analysis and overcoming challenges:

1. **Data Analysis**: I successfully extracted 500 sessions, each with up to 400 comments. However, our efforts were limited by TikTok's blocking mechanisms, preventing us from accessing a larger dataset.

2. **Learning Experiences**: Throughout this phase, I gained valuable insights into using the request library for making HTTP requests, working with proxies in code, and overcoming web scraping challenges posed by large internet companies.

3. **RapidAPI Usage**: We continued to utilize RapidAPI to extract TikTok data based on keywords, including session data such as comments, likes, language, and usernames.

4. **Cyberbullying Identification**: I manually reviewed 20 sessions extracted based on cyberbullying keywords to determine if they contained a significant percentage of cyberbullying comments. Less than half of these sessions were identified as 'cyberbullying' sessions.

5. **Keyword Refinement**: We expanded our list of keywords to enhance the efficiency of selecting social media posts containing cyberbullying.

6. **TikTok Insights**: Our experiences highlighted the challenges of extracting data from TikTok and provided insights into TikTok's anti-cyberbullying policies.

## Semester 3: Exploring Reddit and Comparative Analysis

In our final semester, we expanded our scope to explore Reddit and conducted a comparative analysis of data extraction methods:

1. **Reddit Research**: We conducted research on Reddit, its data structure, and methods for obtaining Reddit data.

2. **API Exploration**: We learned about two Reddit APIs, PushShift and PRAW, which contain Reddit data.

3. **Presentation**: We presented our findings, including comparative insights, using PowerPoint presentations.

4. **Data Extraction on Reddit**: Collaborating with team member Monika Purohit, we performed data extraction tasks on Reddit using PushShift and PRAW.

5. **Comparative Analysis**: We used a Jupyter Notebook script in Python to compare the data structures, data quantities, and overall efficiencies of the two Reddit APIs.

## Conclusion

The BullyBlocker project involved extensive research, data extraction, and analysis efforts, on all platforms, but I primarily focused on TikTok and Reddit. Our work aimed to uncover and address instances of cyberbullying in social media platforms, and we encountered challenges and learning experiences throughout our journey. The project continues to evolve, and we are dedicated to its ongoing success.

**Note**: The final task of generating surveys and labeling sessions for cyberbullying detection is still in progress and is expected to be completed by other team members, since I graduated from Arizona State University.
