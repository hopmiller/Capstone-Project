<!-- Analyzing Spotify Reviews with NLP -->
## Analyzing Spotify Reviews with NLP

Spotify has a large number of reviews on the app stores. These reviews include feedback on how the product is working and whether or not customers like it. By using a dataset of Spotify reviews and ratings from the app store, we will be determining whether the review is positive, negative, or neutral as well as testing the accuracy of the rating using NLP, specifically the Multinomial Bayes model. The model to test the ratings has an accuracy of 67% while the model to test the sentiment of the review has a accuracy of 80%.


![alt text](Spotify_logo_without_text.svg.png)


<!-- Business Understanding -->
## Business Understanding

Spotify was created in 2006 in Stockholm, Sweden by Daniel Ek and Martin Lorentzon. The idea was to create a legal way for users to stream music. Today, Spotify has generated over $9 billion in revenue and has over 180 million subscribers.

Source: [BusinessofApps](https://www.businessofapps.com/data/spotify-statistics/)

An app as popular as Spotify will have hundreds of reviews per day. The reviews give unbiased insight into how customers like the platform, app, and updates. By using NLP, the company can quickly identify common pain points of customers, or things that the customers are enjoying.

### Dataset

The dataset used was collected from scraping the reviews off the of the Google Play Store. It includes over 61,000 customers reviews. Each entry includes a timestamp. the review, the rating given by the customer and replies. For this research, the review and rating were prioritized. It should be noted that the rating was done on a scale of 1 to 5, 5 being the highest. 


<!-- Modeling and Evaluation -->
## Modeling and Evaluation

The first model created classified what the review was rated based on the review itself. This was done by using a Multinomial Naive Bayes model. This model performed with 67% accuracy. The next model I created was also a Multinomial Naive Bayes model. This time, I created a sentiment tag for each review. The sentiment tag was based on the rating. If the rating was a 1-2, it was tagged "negative", if the rating was 3, it was tagged "neutral". If the review was rated a 4-5, it was tagged "positive". The model then tested the accuracy of the classification. It predicted the sentiment of the review based on the review left. This model had an 80% accuracy.

To give Spotify further results, the reviews for positive and negative sentiment were analyzed using Bag of Words. Frequently occurring bi-grams for each sentiment type were pulled. The analysis was performed on the data from the Sentiment Analysis Model because that model had a higher accuracy. 

<!-- Conclusion -->
## Conclusion

I would recommend that Spotify use this model when analyzing customer reviews. The sentiment analysis model performed with the highest accuracy and therefore would be the top choice. The ratings classification model had an above average accuracy score as well, so I would not deter from its use either.

Spotify can use the information from the Bag of Words results to see what is commonly being talked about in positive and negative reviews. It allows a snapshot of the information given by users.
