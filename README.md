[Project II.pdf](https://github.com/Nickbohm555/Netflix-Movie-Recommendation/files/6178492/Project.II.pdf)
# Netflix-Movie-Recommendation

WHAT IS THIS HOW DID I MAKE IT?
---------------
This project is a Netflix Movie Recommendation Engine that uses Machine learning algorithms in the 'PDF' above to solve for a predicted movie rating 'r' of user 'U' for a specific movie 'm'. As of now, I am able to get an predicted rating of around 80-85 Percent which is quite good considering the ratings are a value beween 1-5. That means if I want to know what user 200 will think of movie number 22, if the real prediction of user 200 is 4, I will get a prediction between 3.25 and 4.75. 

Here is how I made it:

 First we need to store all of our data from the textfiles. I only put 2 of them in the GITHUB section because all 2,000 would not fit. However, the same concept applies for 2 as with 2000, we simply won't get meaningful results with 2. In order to store the Data, I had to think through what data structures would be most efficient. Efficiency was paramount for this project because we were dealing with large data sets. I had to store the User ID, the specific movies a user rates and their respective ratings for that specifc movie. At first, I used an ArrayList but quickly found out it would take hours to get any results back this way. 
 
 I figured out that storing each specific user in a new USER_ID class would be able to keep track of the user and storing a hashmap within new class created would get a list of movies as the keys and ratings as the values. 
 
 In order to acess the user's info later, I had to make a second Hashmap which had the UserID as the key and the userID class as the value. Now that I could acess all the information I needed, I first had to solve for the Pierson Coefficient which is in the 'PDF' above. 
 
 After solving for the Pierson coefficient, I found the 100 most similar user's to the User by using the MergeSort algorithm to sort to coefficients from smallest to larges and get the UserID of the top 100 P values. 
 
 Lastly, I plugged in another equation from the 'PDF' above which takes a summattion of values pertaining to the 100 closest neighbors and returns a predicted 'r' value of move 'm'.

WHY DID I MAKE THIS?
---------------------
I made this Movie Recommendation algorithm because I have always had an interest in dealing with large data sets and extracting meaningful answers from it. I wanted to challenge myself over the weekend and see if I was able to think through my design structure intellegently enough to get all 2000 textfiles to my stored and get a predicted 'r' value in around 30 seconds.

HOW DO I USE THIS?
-------------------
In order to Compile this code, you have to run it in eclipse or another Java IDE since it is all coded in Java. Make sure to run the main method ('Netflix') for the code to begin or else it won't compile. Also, the code as of now won't produce meaningful data for you unless you get the other 1998 textfiles of data on movie data. One can find this data online somewhere or ask me for it if they are curious about running it.

OPTIMAL DESIGN CHOICES
-----------------------
I discussed my design choices in the 'How did I make it' section of the ReadME text.

FUTURE IMPROVEMENTS
-------------------
I would like the code to compile quicker, perhaps within 10-15 seconds instead of 30+. I would have to study the complexity of the algorithm quite intensly in order to find out how to shave off some seconds. 

I would also like to get closer to 95 Percent accuracy for my predicted R value. Perhaps I would have to use a different ML algorithm or find out what is causing some problems in my accuracy.
