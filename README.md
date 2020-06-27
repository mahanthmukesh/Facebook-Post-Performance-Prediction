# Facebook-Post-Performance-Prediction

A renowned cosmetics brand is spending a good amount in various marketing platforms in order to improve its brand value which in turn increases its sales. The company has been posting various content on its Facebook (FB) page and wants to know how people are reacting to the marketing campaign that are taking place on that page. Company wants to analyse the efficiency of their Facebook page by using the performance metrics provided by Facebook Insights. 

The data is related to posts' published during the year of 2014 on the Facebook's page of a renowned cosmetics brand.

## Data Description

The Data Set contains 
1. Page Total Likes: Total Number of people liked your page (Numeric Data). 
2. Type: Defines if the type of post is a (Web) Link, Photo, Status or a Video (Categorical Data).  
3. Category: Defines to which category a post belongs to: Action, Product, and Inspiration (Categorical Data). 
4. Paid: Defines if the post is a Paid post (Categorical Data). 
5. Post Hour: Which hour of the day was the post published (Categorical Data). 
6. Post Weekday: Which Day of the week was the post published (Categorical Data) 
7. Post Month: Which Month was the post published (Categorical Data) 
8. Lifetime post total impressions: Impressions are the number of times a post from your Page is displayed (Numeric Data). 
9. Lifetime post impressions by people who have liked your page:  Impressions are the number of times a post from your Page is displayed on the people who likes your page (Numeric Data). 
10. Lifetime Post total Reach: The total number of people who saw the post in its lifetime (Numerical Data). 
11. Lifetime post reaches by people who like your page: The total number of people who saw the post in its lifetime and also like your page (Numerical Data). 
12. Lifetime engaged users: Engaged Users are people who clicked anywhere in your posts that generates a story (Numeric Data). 
13. Lifetime people who have liked your page and engaged with your post: The people who engaged with the post which generates a story and also like the page (Numeric Data). 
14. Lifetime post consumptions: Consumptions measure any click on Post content, whether it generates a Story or not (Numeric Data).  
15. Lifetime post consumers: Consumers are the total number of people who have consumed your post(Numeric Data). 
16. Comments: Total Comments for the post (Numeric Data). 
17. Likes: Total Number of Likes for the Post (Numeric Data). 
18. Shares: Total Number of people who shared the Post (Numeric Data). 
19. Total Interactions: Sum of Total Likes, Comments, Shares (Numeric Data)

## Domain Knowledge


#### Impressions:
After a post is posted on our page, it is displayed on the time line of most of the members of our page. This again depends on the previous level of engagement of the user on the page. If a user who is a member of the page, but not active on the page, might have the post displayed at the bottom of his/her time line.

#### Reach:
It is not necessary that if a particular post displayed on a user time line, the user scroll down in the time line and sees the post. (My assumption here is FB might have an algorithm that will decide on which order the post are displayed on a user time line). Suppose, let us say the user has viewed the post In his time line, that means that the post has reached the user. Else it would just remain as “Impression”(the above metric) and is not reached to the user. 
There is a serious confusion between the metric “Engaged users” and the metric: “Consumers”.  
Before going into these, we need to define what a “story” is, an “engagement” of a post and what “consumption” is. 

Story: A story is something that is displayed on users time line. That is if a user liked, commented, shared any post the friends of that user will be able to see that this user has liked or commented or shared this post. This is a story. 

Engagement: When any user clicks anywhere on your post that creates a story. This is also counted for De-storying.   

Consumptions: Whenever a user performs any clicks on your post, which creates a story along with some other clicks like, playing a video, viewing a photograph, clicking on the link provided comes under consumptions. 
So, above two are explained here with an example. Say, I have a posted picture as a post, and a user named Bob has like my post. Here Bob has created a story. All of the bob’s friends can see that Bob has liked my post. Hence, Bob has engaged with my post. Another user say, Jack has just viewed the image that I posted by clicking on the image, here Jack did not create any story. None of Jack’s friends will know that he has clicked the picture on my post. Hence jack has just consumed my post post. 

Consumers: These are the people who have consumed my post. 
Engaged Users: The users who have been engaged with my post 
Note that: Always the number of Engaged users will be more than the number of consumers. 

Interactions: This is the sum of total Likes, Shares, Comments received for the post. 

## References
Facebook metrics Data Set https://archive.ics.uci.edu/ml/datasets/Facebook+metrics#
