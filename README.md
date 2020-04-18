# Reddit Posts NLP Classification Model

Mariam Javed, DSI-TOR

### Overview

As an upcoming e-commerce business; StudioM currently only has the capacity to develop an app for one operating system (OS) and is therefore deciding between iOS and Android. We're interested in assessing the trends on Reddit and further understanding what OS people are excited about and are talking about these days. We will use the widely popular and top 10-rated subreddit r/gadgets to analyze trends and determine whether people are discussing iOS or Android more.

---

### Problem Statement

Using the Reddit [Web API: Pushshift](https://github.com/pushshift/api), web scrape posts from the r/iOS and r/Android subreddits to determine unique sentiments and develop a classification model. Apply this model to the scraped r/gadgets posts to better understand which OS is most trending.   

Once we determines the preferred mobile app platform/operating system, we're hoping this information will feed into other key considerations and help StudioM determine how to promote our app and what other key functionalities will be involved. 

---

### Executive Summary

Currently, an average mobile user spends more than 81% of their total mobile usage time on the apps installed on their device. This certainly speaks to the popularity of mobile apps and how much potential they carry to take a business to success.

StudioM, an up and coming ecommerce company, is looking to determine which OS they should be building their first app for - iOS or Android? StudioM is hoping to determine this by better understanding the trends on the ever-popular r/gadgets subreddit and developing a model that will be able to classify whether a post created by a user is iOS or Android specific. 

In order to create this classification model, we scraped 2000 posts from r/iOS and 2000 posts from r/Android using the Reddit Web API Pushshift. Based on our evaluation of 5 different models, the SVM model scored a near perfect 0.99 for both the train and validation datasets. Using this model, we predicted whether a post was iOS or Android specific and therefore determined which OS is "hotter" and trending on the r/gadgets subreddit.

This experiment has helped us determine that the 'Android' OS is significnatly discussed more and trending on the r/gadgets subreddit. StudioM will be using this experiment to support their business decision and move forward with creating an app for Android.

Since our classification model was near perfect, it would be beneficial to pull out some of key sentiments and then run our model without these keywords and see how well it performs in that situation. Is there specific lingo for iOS vs Android if we remove the most common easy-giveaways? Does this lingo help us identify the customers further and therefore also identify avenues for advertising/promoting the app? 

---

### Contents:
- [Data Collection](#Data-Collection)
- [EDA](#EDA)
- [Modelling: Training and Validation](#Modelling:-Training-and-Validation)
- [Modelling: Testing](#Modelling:-Testing)
- [Conlclusion and Recommendations](#Conclusion-and-Recommendations)

--- 
