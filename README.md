Project 3: Web APIs & NLP

### Problem Statement

**Problem Statement**
Reddit is a massive collection of forums where people can share social news and content. Essentially, posts are organised according to subject into user-created 'subreddits'. Members submit content (such as images, texts, and links) to subreddits, which can then be voted up ('upvote') or down ('downvote') by other members.

Since the COVID-19 pandemic in 2019, many news reports reveal that there has been a rapidly growing interest in pet ownership.
More people have expressed interest in adopting or fostering dogs and cats for various reasons - such as for companionship during circuit breaker or ease of caring for pets due to work-from-home arrangements.
 
Introducing "CatDog" - a solutions provider company in the Pet Industry. CatDog has outsourced us data scientists to 
* 1. Examine the topics of interest/needs of these new dog and cat owners.
* 2. Provide relevant suggestions on creating new services for dog and cat owners. 

**Goal of this project**
* To scrape relevant subreddits and find out the interests, the needs and the wants of dog and cat owners. 

### Data Collection

- Scrap 10000 post from each subreddit
- Be careful not to overload the server by introducing breaks in between.
- Ensure we have sufficient data for analysis
- Run a quick tokenizer to identify if the keywords are relevant.

---

### Data Cleaning and EDA

The following will be done during Data Cleaning:
- Remove and extract emoji to a new column
- Remove and extract hyperlinks to a new column
- lower case
- Remove numbers
- Remove foreign languages

The following will be examined during EDA:
- Distribution of Title Lengths and Number of Words
- Distribution of new feature emojis
- Examine the top features for each subreddit

---

#### Types of Model

The type of models to be used will be an NLP model followed by a classification model. The NLP model will split the text scrapped from the subreddit and the classification model will be use to predict which subreddit the posts came from.

The NLP model to be deployed in this project is Countvectoriser.

Our team aims to test out a the following classification models.
* Random Forest Classifier
* Extra Trees Classifier
* Logistic Regression
* Multinomial Naive Bayes
* AdaBoost Classifier
* KNeighbors Classifier
* Bagging Classifier

Out of the above models, we will pick the top 2 to optimise and finally pick the best model for production. 

After production, our team will pull the top 20 features of each of the target variable to examine the interest, needs and wants of cat and dog owners.

---

### Conclusion

Our team manage to reached an accuracy score above 90% and able to provide 5 business recommedations for each subreddit.

---

### References

1. https://www.reddit.com/r/cats/
2. https://www.reddit.com/r/cats/
