# Project 3: NLP on Reddit Posts - r/apple and r/samsung

### Overview
This project focuses on NLP modelling using reddit posts from r/apple and r/samsung.

### Background
Apple was created in 1976, by Steve Jobs, a 21-year-old San-Francisco-born hippie, together with Steve Wozniak. But, Wozniak was the person who first built the Apple product called ‘Apple I'. However, by 1997, Jobs led Apple through a massive growth period when he launched iMac, MacOS10, iPod, and iTunes. But it was the iPhone, which launched on 29 June 2007 that overtook the market share. Since then, Apple sold around 2.8b smartphones to date, including 242m devices, last year alone in 2022.

Samsung was founded in 1938 by 28-year-old Lee Byung-Chull. Initially, Samsung was a small trading company dealing in dried fish and noodles. But with the expansion to numerous industries including textile and financial services, Samsung found its golden goose in the late 1960s in the electronics business. There was immense growth in the 1970s and 1980s in its semiconductor business. But, on 29 June 2009,  two years after the iPhone was launched, Samsung introduced the ‘Samsung Galaxy’, its first smartphone.  Since then, Samsung has sold 2b smartphones, and 272m smartphones just in the past year in 2022.

source: https://hellostake.com/nz/blog/stake-updates/head-to-head-apple-vs-samsung

### Problem Statement
- An advertising agency would like to do a marketing campaign to increase the market mindshare for Samsung products in particular mobile smartphones and in turn drive up sales. While Samsung is one of the top leads in the smartphone market share worldwide at 23%, Apple is close behind.
- As part of the marketing campaign preparation, the agency would like to understand the brand mindshare of its products from the internet particularly in the user-generated-content (UGC) domain such as social media channels ie facebook, instagram, twitter and review channels such as tech.radar,trustedreviews.com etc. They were tasked to scrap through all the UGC channels from twitter, facebook, instagram, amazon, reddits to explore and discover what consumers are talking about Samsung; understand the word associations and topics of interest for Samsung consumers.
- The marketing team approached the task with the manual laborious approach of cut-copy-paste from the respective UGC channels and classified them according to its respective buckets i.e. Samsung and its competitors Apple, Oppo etc.
- This approach took too much time which was better spend on creating the most effective marketing mix for the campaign, talking to stakeholders, designers etc. 
- To resolve their problem, the marketing team approached the data science team for help; and the data science team decided to create a simple NLP model that would help the marketing team in saving time. 
- To kick-start, they have identified r/samsung (sub-reddit of samsung) to build an NLP machine learning model and apply it to other UGC channels, with r/apple as its model comparison. 
- The goal is on information retrieval on user generated content across all UGC channels particularly Samsung products. The intent is to scrape all the comments, posts and reviews related to Samsung and place it in the correct Samsung bucket. After this task 1 classification, the 2nd task is to look through all the Samsung posts, reviews etc and deep dive and understand the word associations and topics of interest for Samsung consumers; and with these insights create an effective marketing campaign.
- In summary, the machine learning model is tasked to correctly identify content that is Samsung related and place them in the right label category i.e. "Samsung"; to meet the goal of task 1 classification. This would save the marketing team time on the laborious manual process of classifying the content across all UGC channels. 

---

### Brief Summary of Analysis
From the analysis, the following points were discovered:
1. From the top words in the most upvoted and commented posts from the apple and samsung reddit posts it shows that under the top samsung commented posts, the word 'apple' and 'iphone' are frequently used. This shows that amongst the samsung consumers in the samsung reddits, there is a comparison of samsung products with apple products. However, within the apple most upvoted and commented posts, there is no mention of samsung products, or any samsung related words such as s23, or ultra. This can be infered to show that apple consumers are more 'silo' or focused on the apple products itself and see no value in comparing themselves against samsung. 

2. Also, after data processing (i.e. removing stop words, tags, special characters and digits) in the apple corpus, the key words show consumers seeking advice on a daily basis, talking about the features and app. On the samsung corpus, the key words show consumers are more concerned about the phone, screen, battery, camera and the ultra phone model. From samsung, it shows a more diverse range of topics discussed as compared to the apple corpus.

3. Some common words between both samsung and apple are update, phone, app/s,iphone, day, year, device highlighting that these words while they dont specifically point to either a samsung or apple posts, they should be excluded from the modelling stage to avoid label misclassification. This also shows that both reddits share high common words.

---

### Models Used
The following Models were used:
1. Logistic Regression with tf-idf;
2. Naive Bayes with count vectorizer;
3. Naive Bayes with tf-idf

---

### Conclusions and Recommendations
Based on the different models, it concludes that the naive based tf-idf model is better at meeting the samsung marketing team's task 1 classification of classifying samsung post into to the correct bucket. The goal is to achieve a high recall where the True Positive posts (samsung posts) are maximised and the False Negative posts are minimised. This is to ensure that all the actual samsung posts are in the samsung bucket. Hence, it is recommended for the data science team to deploy this model as a start, and if required to train it further to meet their task 1 classification.