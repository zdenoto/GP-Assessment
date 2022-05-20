# GP-Assessment - Reddit Sentiment Analysis

**Intro** - Everyday millions of people use Reddit.com, and is one of the top most visited websites in the world. This sentiment analysis looks at the GoPro subreddit to help track the number of subscribers for the subreddit, as well as determine if a post is positive or negative. With the results of this, we can track how positive or negative the posts are overall. The results of this could lead to a deeper dive to determine if there are issues with software or certain products to help out customers. 

**Notes when running code** - Reddit API - The reddit API provides an access_token once every 24 hours to pull data with. If you run all line of the code mutliple times within the 24 hour period you will get an error when trying to run it after the first time. After the first time, you will have to paste the access_token from the first time running it as the variable 'access_token' to get the code to run fully. This is in the code as well to help fix the issue.

**Tools** - Python

**Data** - Link for the dataset: https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment?resource=download

**Methods/Evaluation/Techniques** - API, Visualizations, Modeling

![image](https://user-images.githubusercontent.com/105872301/169599721-48e685da-c862-4ce1-b0d5-10ac73955c91.png)

![image](https://user-images.githubusercontent.com/105872301/169599918-d60c0499-6525-46d7-b5c1-0150efa143b0.png)

![image](https://user-images.githubusercontent.com/105872301/169600045-8ac88891-1257-45b7-bfd4-8c5ea53872b9.png)

![image](https://user-images.githubusercontent.com/105872301/169600140-4ba78991-a2dc-4bbc-9542-c1c67dabd382.png)

![image](https://user-images.githubusercontent.com/105872301/169600194-195a107a-4abb-4726-a198-283bfdc052b8.png)

![image](https://user-images.githubusercontent.com/105872301/169600287-17f6f1e7-7bb4-464c-8987-e77c0c2b426a.png)

![image](https://user-images.githubusercontent.com/105872301/169600345-b8ea8e47-29f1-4334-b1b5-ae078c484a62.png)

**Assumptions** - Reddit Data - Some Reddit API data doesn't have time attached. In this analysis for tracking the number of subscribers, I used a random number going back over a year to track the subscribers. In an ideal world, we would have a script pull the number at the same time daily and keep in in a database. I also only looked back to the last 100 reddit posts, ideally we would store the unique id's in a database to access more posts historically. This would help with the machine learning aspect as well.

Positive and Negative Data - The dataset used to determine if a post was positive or negative used a dataset from a twitter dataset instead of using reddit posts or data from the GoPro subreddit. With more time and data, we would ideally use GoPro posts and determine if they are positivie or negative and manually label the data ourselves to train the model.

**Conclusion** - In conclusion, it appears that at the moment in the past few days there are more negative reddit posts in the GoPro subreddit. With more data, we could track the results over a longer period of time to determine if this current amount of positive and negative posts are increasing or decreasing. We could look into the commonalities of the posts to see if there are issues with GoPro products and what the customers feedback are for their products. With fixing these real-world problems, we could potentially fix issues before customers reach out to the company and increase customer satisfaction and customers can feel more GoPro is listening to their customers. With more time and data, the results would only get more accurate as the machine learning algorithm would learn based on specific GoPro data as opposed to the twitter data that was needed for this assessment.
