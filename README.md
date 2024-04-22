#Recommendation Algorithm  
Calculate the distance from other users through collaborative filtering.  
If the number of users is insufficient and the number of recommendations is less than 15,  
it will automatically fill in a part from all unrated TV shows in descending order of views.  

##User-Based Recommendation
Users need to rate TV shows. Calculate the similarity based on the rated part of the user. If the user has not rated or there are no other users, return in descending order of views.
Calculate the distance between users through the Pearson algorithm and find the closest N users. Return the TV shows rated by these users (and unseen by the user to be recommended).
###Item-Based Recommendation
Calculate the similarity matrix of items: https://www.jianshu.com/p/27b1c035b693
Traverse the items rated by the current user and calculate the similarity distance with unrated items.
Sort by similarity distance and return.
