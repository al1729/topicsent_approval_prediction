# math189r_final_project
A project that I worked on with Justin Jiang. We used topic modeling, text sentiment analysis, and an LSTM predictive model to predict President Trump's approval rating solely based off of sentiment analysis of news articles.

Data was sourced from All The News 2.0 (https://www.datasetlist.com/), an online repository containing 2.7 million articles. To build our topic sentiment analysis model, we relied on the Natural Language Toolkit's VADER Sentiment analysis tool, as well as Amazon Comprehend's topic modeling score, to calculate a compound sentiment score for Donald Trump and Joe Biden for each topic in our topic model. This allowed us to identify strong and weak topics for each candidate, corresponding to policy areas in which they were viewed as more competent in. We found that Trump rated especially highly in Middle Eastern politics, abortion, and sports, while Biden was strongest in European politics, American-Russian relations, and families.

We then used Tensorflow to build an LSTM predictive model that took as inputs Trump's sentiment scores for each topic model for each day of his presidency. We then found historical daily approval rating data from FiveThirtyEight (https://projects.fivethirtyeight.com/trump-approval-ratings/?cid=rrpromo) and trained an LSTM to predict future approval ratings given our topic sentiment scores.

More details can be found in our writeups (located in the repository).


