# Airline-Tweets-Sentiment-Analysis---Natural-Language-Processing
Analysis and classification of airline tweets into positive, negative and neutral.

<b>Business Case?</b><br>
We live in the times of the internet and social media, we turn to the internet for almost anything, from deciding which restaurant to eat from, to getting a gift for your neighbour. It becomes increasingly important for organizations around the globe to understand the image of the companies potrayed on the internet to it's potential buyers. We have made one such effort to understand the sentiments of people using the services of the airline industry. This project can be further extended to other social media websites like Instagram, Facebook ... and also other sectors like hotel industry, restaurants, cab services, food delivery partners, and much more. Things like tweets, comments and posts are no longer just an experience that a person shares but have become a uncensored review box for buyers and customers looking for services all around the world.  

The project is divided into 3 main parts:
1) Initial Data Load and Exploratory Data Analysis
2) Data Pre-processing and Vectorization
3) Machine learning modeling and Model Evaluation
<br>

<b>Initial Data Load and Exploratory Data Analysis-</b><br>
The data is loaded using a csv file. The data set contained 219600 tweets and other supplementary information like tweet id, sentiment of the tweet, the confidence associated with the sentiment, tweet location, the date of the tweet, the timezone from which the tweet was tweeted and so on.
<br>
The tweets are associated to 6 major airlines namely - Virgin America, United, Southwest, Delta, US Airways and the American.
A huge majority of these tweets have come from the United States. All of these tweets are from the month of February, 2015.
<br>
Looking at the retweet counts of each of these tweets, these tweets belonged to individuals with a common popularity status, not famous or influential individuals.
<br>
The main reason to focus on the audience, was to understand the lingo on tweets, we are building our Machine Learning Model on.
<br><br>
<b>Data Pre-processing and Vectorization -</b><br>
The main aim of this step was to get rid of words, which added no paritucular functional or informational meaning to the tweet text.<br>
<b>Step 1-</b> We started by running blocks of regualar expressions to remove Emojis, Symbols, Pictographs, Transport and Map Symbols.<br>
<b>Step 2-</b> In the next stage we removed links and other symbols like #, which didn't convey any informational meaning.<br>
<b>Step 3-</b> After that we converted all the text to lower characters and removed stop words<br>
<b>Note:</b> Stop words are commonly used words in the english language, which do not carry significant functional information. E.g. - is, was, are, I ...
<br>
<b>Vectorization</b> - At this stage we converted the remaining part of the tweets, into a matrix, with values calculated based on the repetition of words in a particular tweet and number of tweets with those words in it.<br>
<b>Note: </b>Word Embeddings or Word vectorization is a methodology in NLP to map words or phrases from vocabulary to a corresponding vector of real numbers which used to find word predictions, word similarities/semantics. The process of converting words into numbers are called Vectorization.<br><br>
<b>Machine Learning Modeling and Evaluation -</b><br>
The first step was to form a train/test split in a 80:20 ratio.<br>
For the actual modeling, we built a Random Forest based classifier.<br>
The accuracy associated with it is 75.82%, which is supported by classifying 2928 tweets.







