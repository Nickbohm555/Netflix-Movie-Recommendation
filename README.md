[Project II.pdf](https://github.com/Nickbohm555/Netflix-Movie-Recommendation/files/6178492/Project.II.pdf)
# Netflix-Movie-Recommendation

Takes in over 500,000 users and given the data in text files, comes up with a movie recommendation and rating for respective movies and users. The data structure I mainly used to solve this machine learning problem is HashMaps. It worked quite well because ArrayLists take far too long to loop through and make dynammic changes when looking over 2000 files and over 500K ratings.

I completed this difficult problem in 3 days over the course of 15+ hours coding and designing. Given 2,000 textfiles with each textfile representing a movie, each textfile including several hundred users and several hundred ratings, predict if a given user would enjoy a given movie. First, I had to find a way to store all this data in one place so I would not have to constantly loop thorugh each textfile multiple times, but rather only once. To do this, I stored each individual user to a "UserInfo" class which had a given constructor of it's UserID. Within each class I created a HashMap that stored the movie number as a key and the movie rating as the value. 

However, in order to acess these values I had to be able to acess a specific "UserInfo" class. To do this, I created another HashMap, but this time it took in the UserID as the key and the UserInfo class as the value. This way, when i wanted to acess a specific class, all i had to do was enter the key of that class. 

Storing these values of each user, movie number and coresponding movie rating, I plugged these values into a plethora of different equations given by the PDF above to solve for which other users were most similar to a given user in terms of what movies they liked. neighbors, I used the mergeSort algorithm to rank these users in terms of top 100 most similar neighbors. After doing this, I plugged into another equation above in the PDF to get the predicted rating of a user for a given movie.

Quite a challenging and thrilling weekend project.


\
