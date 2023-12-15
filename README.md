FINAL TASK

Make a project and implement spring security with JWT, restrict access for these APIs as they
can not be accessed by anyone that is not authorized .Save userdetail and dateTime of when the
token is created, set 10 minutes timeout for JWT, it must expire after 10 min and that user can
not get data when the token is expired.

Task1. create an API in which you will pass the JWT token and retrieve the values
saved in that token with it's expiration time.

Task 2.The Task Will be, the REST API contains information about football matches
.The Provided API allows querying matches by year. The Task is to get the number of
matches for a given year that ended in a draw. A match is drawn when both teams
scored the same number of goals.
To access the collection of matches played in a given year, perform an HTTP GET
request to
https://jsonmock.hackerrank.com/api/football_matches?year=2011&page=1.
Each match record has several fields:
1. competition : a string denoting the name of the competition.
2. year : an integer denoting the year the match took place .
3. team1 : a string denoting the name of the first team in the match.
4. team2 : a string denoting the name of the second team in the match.
5. team1goals : a string denoting the number of goals scored by the team1 in the
match
5. team2goals : a string denoting the number of goals scored by the team2 in the
match

NOTE:- * request for these two apis should only be processed if the token is valid , if
not return an appropriate response.
* divide these api's based on rules and roles via spring security, one role can
only access the Task 2 api and the other role can access both Task apis.
* the class need to be used to call the REST API will restTemplate and the
rest api call should be done in seperate thread.
* the resposne for Task2 should be delayed by the 3-6 seconds randomly.
