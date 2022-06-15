# Metis Natural Language Processing Project
## Did the COVID-19 pandemic shift the public perception of bats?

*Abstract:* Bat Conservation International is a nonprofit that works to conserve the worlds bat species. They are interested in how the COVID-19 pandemic has shifted public perception of bats. They plan to use this information to inform their outreach efforts to build support for their work. This analysis showed, that while the percentage of negative tweets did increase with the arrival of COVID-19, it only rose a few percentage points, from 21.35% to 26.57%.

*Design:* I performed topic modeling on over 19,000 tweets about bats to understand the primary themes in what is being communicated about regarding these animals. I removed hashtags, URLs, mentions, and punctuation from the tweets. I then lemmatized the tweets and filtered out non-English words using NLTK’s English word library. I then created a document-term matrix and used non-negative matrix factorization to identify topics and the words associated with those topics. After inspecting the results, I labeled the three resulting topics as related to (1) wind turbine development and its impacts on bats, (2) human wildlife disease transmission, and (3) habitat for bats. I then identified the primary topic present in each tweet and looked at how the prevalence of those topics changed over time. I also performed a Vader sentiment analysis to understand if tweets became more positive or negative overall after the start of the COVID-19 pandemic. 

*Data:* I scraped 19,443 tweets that contained the words “bat” and “wildlife” from between January 1st, 2019 and June 9th, 2022.

*Algorithm:*

*Tools:*
- Pandas and Numpy for data manipulation
- Twint for scraping tweets
- spaCy for lemmatizing words
- NLTK for filtering out non-English words and Vader sentiment analysis
- scikit-learn for document-term matrix creation and non-negative matrix factorization
- Scattertext and WordCloud for term visualization

*Communication:*
- A Scattertext visualization of terms can be found here
- Slides summarizing the analysis and relevant findings can be found here
