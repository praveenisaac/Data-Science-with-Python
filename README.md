# Data-Science-with-Python
Simplilearn- Project 2 - Movielens Case Study

DESCRIPTION

Background of Problem Statement :

The GroupLens Research Project is a research group in the Department of Computer Science and Engineering at the University of Minnesota. Members of the GroupLens Research Project are involved in many research projects related to the fields of information filtering, collaborative filtering, and recommender systems. The project is led by professors John Riedl and Joseph Konstan. The project began to explore automated collaborative filtering in 1992 but is most well known for its worldwide trial of an automated collaborative filtering system for Usenet news in 1996. Since then the project has expanded its scope to research overall information by filtering solutions, integrating into content-based methods, as well as, improving current collaborative filtering technology.

Problem Objective :

Here, we ask you to perform the analysis using the Exploratory Data Analysis technique. You need to find features affecting the ratings of any particular movie and build a model to predict the movie ratings.

Domain: Entertainment

Analysis Tasks to be performed:

Import the three datasets
Create a new dataset [Master_Data] with the following columns MovieID Title UserID Age Gender Occupation Rating. (Hint: (i) Merge two tables at a time. (ii) Merge the tables using two primary keys MovieID & UserId)
Explore the datasets using visual representations (graphs or tables), also include your comments on the following:
User Age Distribution
User rating of the movie “Toy Story”
Top 25 movies by viewership rating
Find the ratings for all the movies reviewed by for a particular user of user id = 2696
Feature Engineering:
            Use column genres:

Find out all the unique genres (Hint: split the data in column genre making a list and then process the data to find out only the unique categories of genres)
Create a separate column for each genre category with a one-hot encoding ( 1 and 0) whether or not the movie belongs to that genre. 
Determine the features affecting the ratings of any particular movie.
Develop an appropriate model to predict the movie ratings
Dataset Description :

These files contain 1,000,209 anonymous ratings of approximately 3,900 movies made by 6,040 MovieLens users who joined MovieLens in 2000.

Ratings.dat

Format - UserID :: MovieID :: Rating :: Timestamp


Field:	Description
UserID:	Unique identification for each user
MovieID:	Unique identification for each movie
Rating:	User rating for each movie
Timestamp:	Timestamp generated while adding user review
![image](https://user-images.githubusercontent.com/71750093/154732305-865896f7-0575-4fea-ac8b-036a725f75c8.png)

1. UserIDs range between 1 and 6040
2. The MovieIDs range between 1 and 3952
3. Ratings are made on a 5-star scale (whole-star ratings only).
4. A timestamp is represented in seconds since the epoch is returned by time(2).
5. Each user has at least 20 ratings
 

Users.dat

Format -  UserID :: Gender :: Age :: Occupation :: Zip-code

Field:	Description
UserID:	Unique identification for each user
Genere:	Category of each movie
Age:	User’s age
Occupation:	User’s Occupation
Zip-code:	Zip Code for the user’s location


![image](https://user-images.githubusercontent.com/71750093/154732743-46758461-b75c-466c-b3ef-771bb468f348.png)


All demographic information is provided voluntarily by the users and is not checked for accuracy. Only users who have provided demographic information are included in this data set.

1. Gender is denoted by an "M" for male and "F" for female.
2. Age is chosen from the following ranges:


![image](https://user-images.githubusercontent.com/71750093/154734117-0ebc68c8-d719-4e0a-b336-264b315f0d87.png)




Occupation is chosen from the following choices:

Value 	Description
0	other or not specified
1	academic/educator
2	"artist”
3	clerical/admin"""
4	college/grad student
5	customer service
6	doctor/health care
7	executive/managerial
8	farmer
9	homemaker
10	K-12 student
11	lawyer
12	programmer
13	retired
14	 "sales/marketing"
15	scientist
16	 "self-employed"
17	technician/engineer
18	tradesman/craftsman
19	unemployed
20	writer”
![image](https://user-images.githubusercontent.com/71750093/154733057-a3bbd498-bf13-43e3-9b8b-4ccd28bed1da.png)


Movies.dat

Format - MovieID :: Title :: Genres

Field:	Description
MovieID:	Unique identification for each movie
Title:	A title for each movie
Genres:	Category of each movie
	
![image](https://user-images.githubusercontent.com/71750093/154733197-b8adf32d-f939-44f7-9d7b-ea420df87762.png)
 
1. Titles are identical to titles provided by the IMDB (including year of release).
2. Genres are pipe-separated and are selected from the following genres:


1. Action.
2. Adventure.
3. Animation.
4. Children's.
5. Comedy.
6. Crime.
7. Documentary.
8. Drama.
9. Fantasy.
10. Film-Noir.
11. Horror.
12. Musical.
13. Mystery.
14. Romance.
15. Sci-Fi.
16. Thriller.
17. War.
18. Western.


Some MovieIDs do not correspond to a movie due to accidental duplicate entries and/or test entries

Movies are mostly entered by hand, so errors and inconsistencies may exist
